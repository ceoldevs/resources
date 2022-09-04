# Rendering techniques

To render the content on the website, there are many ways 
to achieve this depending upon the requirement. The three
famous techniques are Server Side Rendering (SSR), Static
Site Generation (SSG) and Client Side Rendering (CSR).

## SSR v SSG v CSR

Below are the differences between all the three above 
rendering techniques currently used

- SSR: In case of Sever Side Rendering, the html and css 
are built right when the request is made by fetching from 
any data sources mentioned and sending it to the server.

- SSG: Instead of building the html and css when the 
request is made unlike SSR, in Static Site Generation, 
the data is fetched from the data sources at the building 
step of the application and the same html and css files are
served to the client. To make any updates, the application 
should be rebuilt again.

- CSR: Client side rendering is the often method you have 
noticed if you havent worked with any meta framework where 
the javascript is sent to the client on request at first 
and the client directly fetches from the data sources from 
client side unlike in the above methods where there is an 
intermediate server which fetches data from data sources.

SSR and SSG are called as pre-rendering techniques as the 
content is rendered before sent to the client. 

Both SSR and SSG work well for content driven websites 
where the content is static and also helps in SEO 
indexing as any content driven application would require. 
Examples of these websites would be blog sites and 
e-commerce websites.

SSG would work very well with personal blogs or portfolio 
pages as the content doesnt update that often and you will 
be the only person updating the content.

But if authentication is required, even blog applications 
work well with the SSR technique. E-commerce website content
updates quite often and also require SEO features and hence,
SSR will work good.

CSR is a concept used directly with applications like 
dashboard which require realtime updating of the content and
also doesnt require SEO indexing compared to a blogging 
applications.

## Hydration and SPAs

To achieve features like routing, CSR based apps use a 
concept called Single page application where there is no 
router or a router intercepting the route requests of 
server at the client side and using javascript to change 
the data. A good example of this is Gmail where when a mail
is opened or a different category is used, the application 
instantly loads without a reload of page. This is achieved 
as there is no request to the server for the page but 
instead, the javascript in client directly contacts the data
source and renders as HTML.

Although major parts of rendering of application can be 
handled in the server with SSR, some components require 
loading the content to be updated realtime (like comments 
section). To solve this, there is a technique called 
hydration where the the HTML and CSS sent by the server 
gets replaced with the javascript which is also sent at a
later time and loads lazily. This allows us to render the 
content and styling to make the site look fast and the 
funtionality is loaded shortly after this.

This loading can be done partially or completely. Frameworks
like Next.js and SvelteKit entirely hyrdates the website and
provides an SPA routing which provides best of both worlds 
from CSR and SSR.

checkout next.js hydration in SSR section - 
https://nextjs.org/learn/foundations/how-nextjs-works/rendering

But entirely hydrating the client requires to fetch extra 
data which will slow down the website. To solve this issue, 
we have Partial hydration concept used by astro islands where 
only the conponents that require javascript is hydrated 
allowing to ship as minimal javascript as possible.

check out astro islands - 
https://docs.astro.build/en/concepts/islands/

For more detailed pros and cons, check this blog - 
https://medium.com/nerd-for-tech/compare-and-contrast-csr-ssr-and-ssg-in-nextjs-58e3caf2e15e

Credits - Fireship.io

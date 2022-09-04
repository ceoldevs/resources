# Learning material for `Astro` meta framework

Astro is a meta framework that can be used with mix of many
libraries (currently supports: svelte, react, preact, vue,
solid)

## So what are meta frameworks?

Till now you may have only worked with the so called JS
libraries like react, svelte, vue etc. But these are only
component libraries providing a method to manage the 
application with a component approach.

But when it comes to real application. This will be just a 
part of the bigger picture. We require many other parts like
Routing, Data fetching, Rendering, Infrastructure, 
Performance and Scalability. To take care of this, we have 
the meta frameworks.

One of the famous meta frameworks in the market is Next.js 
which uses react for component management and on top of 
react, added a routing (filepath based routing), 
Rendering techniques (SSG, SSR. Will talk in the next 
sections), and ability to deploy the frontend in 
edge functions like vercel (Next.js is supported by 
Vercel team. Vercel provides us runtime environment to 
launch many frontend applications in a serverless 
fashion).

Astro is another famous framework created recently and 
gained its popularity with the claim to ship 
**zero javascript** in the client and comes with an 
island architecture of components.

## Why zero javascript?

Javascript is a powerful tool but browsers require to run 
the javascript to use its power. Running JS uses resources 
and time significantly enough to reduce the user experience
because of time.

So what is the solution? Ship no javascript.

Well it is not that easy as we do need javascript to do 
some tasks.

To solve this issue, in the recent versions plain javascript 
can be added with the `<script>` tag. But to improve 
efficiency in developer experience, we choose to use JS 
libraries. But what library to choose? Well choose anything.

To learn more about the reason to use astro, check this 
page - https://docs.astro.build/en/concepts/why-astro/

> If you Dont understand rendering techniques like SSR, 
SSG and CSR, Check out resources of 
[rendering techniques](../rendering-techniques.md)

## Astro's Islands Architecture 

If you have learned about any JS libraries (which is 
required to write better code in astro), there is a concept
of components where the sections of the web page are 
divided into components like Navigation, Header, Menu, 
Footer. If we take React.js for example, how many of these
components require reactivity? Stuff like footer and header
may not require to be loaded by javascript. But this is not
hanlded by react.js.

Next JS takes an approach of first rendering the static 
content like these and then **hydrating** the static assets
with JS after client loaded .

This does solve the problem but some of the components 
doesnt require javascript to be hydrated as they are pure 
static content.

To solve this issue, Astro generates the content with zero 
client side javascript. But to have interactivity, we can 
create those certain components with the any library of 
our choice. 

Once the request is served with the HTML and CSS files 
required, we have methods to hydrate the client for the 
required isolated components in multiple ways like loading 
instantly with the client fetching, loading when the client
is idle, loading the component when it is displayed on the 
screen.

Sometimes we may require to share state between the 
component islands. But due to the nature of Astro not taking
the client entirely with javascript and using multiple 
component libraries, astro requires a library agnostic store 
management tool. Nanostores is one state management library 
that provides us state management.

Nanostores - https://github.com/nanostores/nanostores
Nanostores in astro - https://docs.astro.build/en/core-concepts/sharing-state/

To learn more about astro Islands architecture, check this
page - https://docs.astro.build/en/concepts/islands/

Now that you understand how astro works and familiar with 
any javascript library, you can start creating projects in
astro.

check all the features provided by astro here - 
https://docs.astro.build/en/core-concepts/project-structure/

The documentation will be more than enough resources for 
this application. 

To check some examples of the applications in astro, you 
can have a look at the 
[ceol-frontend-fe](https://github.com/ceoldevs/ceol-frontend-fe.git)
repo built using astro 1.0 with tailwind css and SSR 
integrated with API built in golang.

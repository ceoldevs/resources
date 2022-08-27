# Golang Learning Resources

Golang is a fairly new technology developed in google and
considered as a successor of C to solve the issues of the 
modern workloads which lacked with C programming. Golang 
is developed by the same creator of C (Ken Thompson).

## Official Resources

The developers of go has provided a tour of golang with
interactive learning method.

https://go.dev/tour/welcome/1

## Youtube Resources

net ninja has a playlist to learn golang. Here is the link 
for the playlist.
https://www.youtube.com/watch?v=etSN4X_fCnM&list=PL4cUxeGkcC9gC88BEo9czgyS72A3doDeM

# Web Development with Golang.

We are using golang for building web servers. Go philosophy 
focuses on minimalism and therefore using frameworks is not 
a trend followed by the community. 

Go provides it's own `net/http` package providing enough
features and is directly used by many projects.

But after talking with the community, we have decided to 
use `go-chi` package built on `net/http` making it easier 
to develop webservers. (For those who know JS, you can
think of this as an equivalent of express.js). 

For learning go-chi, major dependency is to understand 
how `net/http` works as it plays a major role in the 
underlyings of building a webserver with go (unlike node.js 
where without understanding the node.js http package can 
understand express.js to a certain point).

### Resources

Docs for `net/http` - https://pkg.go.dev/net/http
Docs for `go-chi` router - https://go-chi.io/#/pages/getting_started

If you dont have understanding of how HTTP works and how 
the websites work, here are Mozilla's documents.

- Overview - https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview
- Full docs - https://developer.mozilla.org/en-US/docs/Web/HTTP

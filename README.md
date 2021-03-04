
# Source for my personal profile site 

I just rebuilt my profile [site](https://herrell.dev) with new framework called Svelte. More specifically I am using Svelte's server-side rendering framework called Sapper. Conceptually this is like Angular Universal and React's 	Next which use a node server like express to initially render components on the first call on server. Then use service workers to prefetch content and hydrate more of the application on the front end once it's loaded in the browser. The main difference here is Svelte does not have a runtime nor use a virtual dom.





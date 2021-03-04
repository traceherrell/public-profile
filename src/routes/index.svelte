<script>
	import profile from "images/profile_standing.jpg";
	import { Button } from "sveltestrap/src";

	const scrollTo = (e) => {
		e.stopPropagation();
		if (window) {
			window.scrollTo({
				top: 700,
				left: 100,
				behavior: "smooth",
			});
		}
	};
</script>

<svelte:head>
	<title>Trace Herrell</title>
</svelte:head>

<header class="header">
	<div class="container">
		<div class="row">
			<div class="col-md-6">
				<img alt="Profile" src={profile} class="img-responsive" />
			</div>
			<div class="col-md-6">
				<h2 class="heading">Hello, I'm Trace</h2>
				<p>
					A Software Engineer from the Pacific North West, Seattle
					area. Want to know more about me?
				</p>
				<Button color="secondary" on:click={scrollTo}>Read More</Button>
				<a
					href="https://www.linkedin.com/pub/trace-herrell/66/a84/423"
					class="btn btn-primary"
				>
					<i class="fa fa-lg fa-linkedin" />
				</a>
			</div>
		</div>
	</div>
</header>

<section class="section about-me">
	<div class="container">
		<h2 class="heading">About Me</h2>
		<div>
			<p>
				I have lots of experience building end to end solutions in a
				variety of verticals: healthcare, insurance, e-commerce, real
				estate, education, and <span class="fa fa-bluetooth" />IoT. I’m
				strong in all areas of the stack but in last few years I’ve
				really began focusing more on the middle to front end with
				modern javascript technology like React, Vue, Angular, Kendo UI,
				Node.
			</p>
		</div>
		<div>
			<p>
				As a lifetime learner I'm always interested in technology
				and different approaches to software engineering. I just rebuilt
				this site with new framework calleed Svelte. More specicially
				I'm using Svelte's serverside rendering framwork called Sapper.
				Conceptually this is similar to Angular Universal and React's
				NextJs which use a node server like express to initially render
				components on the first call on server. Then use service workers
				to prefetch content and hydrate more of the application on the
				front end once it's loaded in the browser. The main difference
				here is Svelte does not have a runtime nor use a virtual dom.
				All code is compiled to plain javascript. The other two times
				were built with React and then with Vue. And even though I'm
				Azure certified it's hosted on Gooogle Cloud Platform. Here's
				the link to the <a
					href="https://github.com/traceherrell/traceherrell.github.io"
				>
					source.</a
				>
			</p>
			<p />
		</div>

		<div class="row interest">
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-html5" /> HTML/CSS3
				</h3>
				<p>
					Implement responsive designs for a usable experience across
					desktop, tablet, and phone browsers. Sass, Less, HTML5
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-code" /> Code
				</h3>
				<p>
					Well versed in functional and OO programming. JavaScript,
					C#.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-cloud" /> API
				</h3>
				<p>
					Develop RESTful interfaces that incorporate stateless
					designs, self-descriptive messages and semantic URLs. Web
					API 2.0, NodeJs, Google Map, Facebook Social, AWS Cloud,
					OATH2
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-database" /> Database
				</h3>
				<p>
					Skillful in creating conceptual models based on business
					logic and executing performance tuning on Databases.
					Relational, SQL Server, document storage, MongoDB, TSQL,
					Modeling, Query optimization.
				</p>
			</div>
		</div>

		<div class="row interest">
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab  fa-react" /> React
				</h3>
				<p>
					Implement responsive designs for a usable experience across
					desktop, tablet, and phone browsers. Sass, Less, HTML5
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab fa-vuejs" /> Vue
				</h3>
				<p>
					Well versed in functional and OO programming. JavaScript,
					C#.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab  fa-microsoft" /> API
				</h3>
				<p>
					Develop RESTful interfaces that incorporate stateless
					designs, self-descriptive messages and semantic URLs. Web
					API 2.0, NodeJs, Google Map, Facebook Social, AWS Cloud,
					OATH2
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-database" /> Database
				</h3>
				<p>
					Skillful in creating conceptual models based on business
					logic and executing performance tuning on Databases.
					Relational, SQL Server, document storage, MongoDB, TSQL,
					Modeling, Query optimization.
				</p>
			</div>
		</div>
	</div>
</section>

<style>
	.header .heading {
		font-size: 4em;
		margin-bottom: 0;
	}

	.header p {
		font-size: 2em;
		margin-bottom: 55px;
		line-height: 1.5;
		font-weight: 200;
	}
	.about-me {
		margin-top: 100px;
	}
	.about-me p {
		margin-bottom: 20px;
	}

	.interest {
		margin-top: 75px;
	}
</style>

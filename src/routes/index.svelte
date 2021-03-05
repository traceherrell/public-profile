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
					href="https://www.linkedin.com/in/traceherrell/"
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
				I have several years of experience building end to end solutions in a
				variety of verticals: healthcare, insurance, e-commerce, real
				estate, education, and IoT. I am competent engineer and manager
				comfortable in all areas of the software stack. an in the last
				few years I have really used my experience to help organizations
				build right sized, scalable, and maintainable solutions often
				during times of technical transformations. As an Azure certified
				solution architect and certified scrum master I bring years of
				experience to leading teams and organizations design and build
				new capabilities.
			</p>
		</div>
		<div>
			<p>
				As a lifetime learner I'm always interested in new technology
				and different approaches to software engineering. I rebuilt this
				site with new framework called <a href="https://svelte.dev/">
					Svelte</a
				>. More specifically I am using Svelte's server-side rendering
				framework called Sapper. Conceptually this is like Angular
				Universal and React's Next which use a node server like express
				to initially render components on the first call on server. Then
				use service workers to prefetch content and hydrate more of the
				application on the front end once it's loaded in the browser.
				The main difference here is Svelte does not have a runtime nor
				use a virtual dom. All code is compiled to plain JavaScript. The
				other two times were built with React and then with Vue. And
				even though I am Azure certified it is hosted on Gooogle Cloud
				Platform. Here is the link to the
				<a
					href="https://github.com/traceherrell/public-profile"
				>
					source.</a
				>
			</p>
			<p />
		</div>
		<div class="row interest">
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab  fa-react" /> React
				</h3>
				<p>
					I've built a couple of projects as well as leading new end
					teams. Redux state management, story book componenents
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab fa-vuejs" /> Vue
				</h3>
				<p>
					Introduced Bluetooth to Vue and led the adoption state
					mangement (Vuex) as a design pattern.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab  fa-microsoft" /> .Net Core
				</h3>
				<p>
					Micro services. Queues, Event Sourcing, Repository,
					Dependency injection.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fab fa-docker" /> Docker
				</h3>
				<p>
					Azure container services (ACS), Azure Kubernetes Service
					(AKS), Azure DevOps.
				</p>
			</div>
		</div>
		<div class="row interest">
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-html5" /> HTML/CSS
				</h3>
				<p>
					Implement responsive designs for a usable experience across
					desktop, tablet, and phone browsers.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-code" /> Code
				</h3>
				<p>
					Well versed in functional and OO programming. I primarily
					write JavaScript, and C#. Recently new to Rust
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-cloud" /> API
				</h3>
				<p>
					Develop RESTful interfaces that incorporate stateless
					designs, self-descriptive messages and semantic URLs.
					Apigee, Azure Api Management.
				</p>
			</div>
			<div class="col-md-3">
				<h3 class="sub-heading">
					<i class="fa fa-lg fa-database" /> Database
				</h3>
				<p>
					Relational, Document, Azure SQL Server, Cosmos, Mongo,
					Redis, TSQL, Modeling, Query optimization.
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
		font-size: 1.1em;
	}

	.interest {
		margin-top: 75px;
	}

	.interest p {
		font-size: 1em;
	}
</style>

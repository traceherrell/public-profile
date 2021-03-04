<svelte:head>
	<title>Work History</title>
</svelte:head>


<section class="section resume">
	<h2 class="heading">Resume</h2>
	<div class="container">
		<ul class="timeline">
			<li class="year">2021</li>
			<li class="event">
				<h3 class="heading">Architect/Manager @ T-Mobile</h3>
				<span class="month">
					<i class="fa fa-calendar" />October 2019 - Feb 20021
				</span>
				<p>
					Provided high level solution design, LOE’s, and technical
					guidance to product and delivery teams in the digital
					commerce space. Built POC’s with Serverless framework to
					improve CI/CD Infrastructure as code deployments to AWS.
					<a href="https://t-mobile.com/plans"> t-mobile.com/plans</a>
				</p>
			</li>
			<li class="event">
				<h3 class="heading">
					Lead Software Engineer / Architect @ CFC
				</h3>
				<span class="month">
					<i class="fa fa-calendar" />April 2016 - May 2017
				</span>
				<p>
					Hired and led a team of developers and the organization
					through a technology transformation breaking apart existing
					monolithic CMS, migrating to scalable Azure cloud based
					ecosystem.
				</p>
				<p>.NET Core, React, Ngnx, Azure</p>
				<p>
					<a href="https://www.secondstep.org">secondstep.org</a>
				</p>
			</li>
			<li class="year">2017</li>
			<li class="event">
				<h3 class="heading">
					Lead Software Engineer / Architect @ Bluetooth
				</h3>
				<span class="month">
					<i class="fa fa-calendar" />April 2016 - May 2017
				</span>

				<p>
					Using architectural patterns such as Separation of Concerns,
					Encapsulation, Caching, Dependency injection, MVC, MVVM
					design patterns I significantly improved the design of a
					project currently two years into development. Measured by
					performance, maintainability, and user feedback we able to
					finally launch a successful beta.
					<a href="https://www.bluetooth.com">www.bluetooth.com</a>
				</p>
			</li>

			<li class="event">
				<h3 class="heading">Software Engineer @ John L Scott</h3>
				<span class="month">
					<i class="fa fa-calendar" />Decemmber 2014 - March 2016</span
				>
				<p>
					Complete responsive redesign and implementation for John L.
					Scott's public facing search application as we well as the
					back end broker tools. Built new front end using JavaScript
					MVVM frame works, React, Flux, bootstrap, and google api's
					(map, geography, social).
					<a href="https://www.johnlscott.com/search"
						>www.johnlscott.com</a
					>
				</p>
			</li>
			<li class="year">2015</li>

			<li class="event">
				<h3 class="heading">Senior Developer @ Childrens Hospital</h3>
				<span class="month">
					<i class="fa fa-calendar" />May 2012 – Oct 2014</span
				>
				<p>
					Designed/Implemented a new web application for the IPU,
					replacing the current white board manual process. Used
					Asp.net MVC 5. Razor, Bootstrap, JQuery and Entity
					Framework.
				</p>
			</li>

			<li class="event">
				<h3 class="heading">Senior Developer - Freelance</h3>
				<span class="month">
					<i class="fa fa-calendar" />January 2012 – May 2012</span
				>
				<p>
					Implemented a Cole and Weber designed Facebook application
					for Washington State Lottery. JQuery, CSS, .Net 4.0,
					ASP.Net, SQL server to build the “Group Play” application.
				</p>
			</li>
			<li class="year">2012</li>
			<li class="event">
				<h3 class="heading">Software Engineer at Vertafore</h3>
				<span class="month">
					<i class="fa fa-calendar" />October 2007 – January 2012</span
				>
				<p>
					End to end full stack software engineer and scrum master. 6
					major releases. 100,000+ users.
				</p>
			</li>

			<li class="event">
				<h3 class="heading">
					Software Developer at Childrens Hospital
				</h3>
				<span class="month">
					<i class="fa fa-calendar" />Jan 2000 – March 2007</span
				>
				<p>
					Working closely with executive stake holders I built several
					web applications that focused on improving patient outcomes
					and reducing clinical administrative overhead.
				</p>
			</li>
		</ul>
	</div>
</section>

<style>
	p {
		margin: 1em auto;
		text-align: left;
	}

	.heading {
		margin-top: 20px;
	}

	section {
		margin-bottom: 100px;
	}

	.section .heading {
		font-size: 3em;
		line-height: 1.6;
		margin-top: 0;
		margin-bottom: 30px;
		text-align: center;
	}

	.timeline {
		margin: 0 auto;
		max-width: 700px;
		overflow: hidden;
		height: auto;
		position: relative;
		padding: 0;
		list-style-type: none;
		background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEElEQVQIW2NMTEz8z8gABAAPKwIlXWq1kgAAAABJRU5ErkJggg==);
		background-repeat: repeat-y;
		background-position: 50% 0;
	}

	.timeline .heading {
		font-weight: 700;
		font-size: 1.2em;
		font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
		text-align: left;
		margin-bottom: 0;
	}

	.timeline .year {
		font-size: 1em;
		line-height: 4;
		color: #fff;
		width: 6em;
		border-radius: 50%;
		background: #505050;
		max-width: 4em;
		clear: both;
		margin: 1em auto;
		text-align: center;
		margin-top: 50px;
	}

	@media screen and (min-width: 992px) {
		.timeline .year {
			margin-bottom: 30px;
		}
	}

	.timeline .year + .event {
		margin-top: 50px;
	}

	.timeline .month {
		display: block;
		margin-bottom: 15px;
		color: #aea08b;
		font-size: 0.9em;
	}

	.timeline .month i {
		margin-right: 5px;
	}

	.timeline .event {
		width: 100%;
		margin: 50px 0;
		padding: 1.3em;
		background: #f4f4f4;
		border-color: #bcbcbc;
		text-align: left;
		color: #3c3c3c;
	}

	@media screen and (min-width: 992px) {
		.timeline .event {
			width: 45%;
			margin: 110px 2.5% 50px;
		}
	}

	.timeline .event:hover {
		background: #f4f4f4;
	}

	.timeline .event:hover:after {
		background: #2c3e50;
	}

	.timeline .event:after {
		width: 25px;
		height: 12px;
		border-color: #efefef;
		border-width: 5px;
		background: #95a5a6;
		top: 1.8em;
		left: -29px;
	}

	.timeline .event:nth-of-type(2n):after {
		right: -31px;
	}

	.timeline .heading {
		color: #2c3e50;
		font-weight: 700;
		font-size: 1.2em;
		font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
		text-align: left;
		margin-bottom: 0;
	}

	.timeline.timeline-right .event:nth-of-type(2n) {
		float: right;
		clear: right;
	}

	.timeline.timeline-right .event:nth-of-type(2n):after {
		right: auto;
		left: -29px;
	}

	@media screen and (min-width: 992px) {
		.timeline.timeline-right .event {
			margin-top: 30px;
		}
	}

	.timeline.timeline-left .event {
		float: left;
		clear: left;
	}

	.timeline.timeline-left .event:after {
		left: auto;
		right: -29px;
	}

	.timeline *,
	.timeline :after,
	.timeline:after,
	.timeline :before,
	.timeline:before {
		-webkit-box-sizing: border-box;
		-moz-box-sizing: border-box;
		box-sizing: border-box;
	}

	.timeline .year:first-of-type {
		margin-top: 0 !important;
	}

	.timeline .year + .event {
		margin-top: -1.5em;
	}

	.timeline .event {
		position: relative;
		float: right;
		clear: right;
		width: 45%;
		margin: 10px 2.5%;
		border-radius: 5px;
		list-style-type: none;
		display: block;
		padding: 0.4em;
		background: #fff;
		z-index: 15;
		color: #4d4d4d;
		border: 1px solid #d0d0d0;
		text-decoration: none;
		-webkit-transition: background 0.15s linear;
		-moz-transition: background 0.15s linear;
		-ms-transition: background 0.15s linear;
		-o-transition: background 0.15s linear;
		transition: background 0.15s linear;
	}

	

	@media all and (max-width: 600px) {
		.timeline .event {
			width: 85%;
		}
	}

	

	.timeline .event:hover {
		background: #f6f6f6;
	}

	.timeline .event:hover:after {
		background: #505050;
	}

	.timeline .event:nth-of-type(2n) {
		float: left;
		clear: left;
	}

	.timeline .event:nth-of-type(2n):after {
		right: -5%;
		left: auto;
	}

	@media all and (min-width: 650px) {
		.timeline .event:after {
			display: block;
			content: " ";
			height: 9px;
			width: 9px;
			background: #9d9d9d;
			border-radius: 50%;
			position: absolute;
			left: -5%;
			top: 1.5em;
			border: 2px solid #fff;
		}
	}

	.timeline time {
		display: block;
		font-weight: 700;
	}
</style>

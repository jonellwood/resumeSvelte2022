<script>
	import Hr from '../lib/hr.svelte';
</script>

<main>
	<div class="white-box-in-middle-to-look-like-piece-of-paper">
		<div class="top-div-for-decoration">
			<p class="hidden-text-in-top-div">
				IF YOU CAN SEE THIS TEXT YOU ARE PROBABLY VIEWING SOURCE. PLEASE FEEL FREE TO SUBMIT IDEAS
				TO MAKE THIS BETTER.
			</p>
		</div>
		<div class="container-for-everything">
			<aside class="aside-front-page">
				<h2>Jon Ellwood</h2>
				<span>
					<p>
						21 Monte Sano Drive<br />
						Hanahan SC 29410 <br />
						<a href="tel:843-743-4259">843-743-4259</a><br />
						<a href="mailto:jonellwood@gmail.com">jonellwood@gmail.com</a><br />
						<a href="https://jonellwood.dev">jonellwood.dev</a>
					</p>
					<!-- <p class="silly-note">Can you believe you get this in HTML with no CSS or JS? So cool.</p> -->
				</span>
			</aside>
			<div class="next-to-the-aside">
				<h2 class="objective-h2">Objective:</h2>
				<p class="objective-p">
					To join a team that can leverage my existing experience and continue to grow my skills set
					to benefit both myself and my employer. In my most recent employment I was fortunate to be
					exposed to a multitude of IT related functions allowing to me to get fairly proficient in
					many things. I am now seeking a position that will allow me to become very good at one or
					two things.
				</p>
			</div>
		</div>
		<Hr />
		<div class="experience">
			<h2>Experience</h2>
			<table class="experience-table">
				<tr>
					<th>Company</th>
					<th>Job Title</th>
					<th>Dates</th>
				</tr>
				<tr>
					<td>City of Hanahan</td>
					<td>IT Director</td>
					<td>January 2019 - June 2022</td>
				</tr>
				<tr>
					<td>Hanahan Police Department</td>
					<td>Certified Police Officer</td>
					<td>April 2010 - January 2019</td>
				</tr>
				<tr>
					<td>Berkeley County Sheriff's Office</td>
					<td>Detention Officer</td>
					<td>December 2008 - April 2010</td>
				</tr>
				<tr>
					<td>COMDOC Business Systems</td>
					<td>Sales and Sales Manager</td>
					<td>December 1998 - December 2008</td>
				</tr>
			</table>
		</div>
		<Hr />
		<div class="education">
			<h2>Education</h2>
			<table class="education-table">
				<tr>
					<th>Location</th>
					<th>Degree</th>
					<th>Dates</th>
				</tr>
				<tr>
					<td>SC Criminal Justice Academy</td>
					<td>Class 1 Certification</td>
					<td>July 2010</td>
				</tr>
				<tr>
					<td>Trident Technical College</td>
					<td>Associate Degree in Criminal Justice</td>
					<td>December 2014</td>
				</tr>
			</table>
		</div>

		<Hr />
		<div class="relevant-skills">
			<h2>Relevant Skills</h2>
			<table class="skills-table">
				<tr>
					<th />
					<th />
					<th />
				</tr>
				<tr>
					<td>Office 365 Administrator</td>
					<td>Windows Server 2012 Domain Administrator</td>
				</tr>
				<tr>
					<td>CJIS Compliance Officer (LASO & CLO)</td>
					<td>Wordpress Site Administrator</td>
				</tr>
				<tr>
					<td>3CX Administrator</td>
					<td>Woodworking</td>
				</tr>
			</table>
		</div>
		<Hr />
		<div class="education">
			<h4>Select the Review tab for a list of online courses & certifications I have completed</h4>
		</div>
	</div>
</main>

<style>
	a {
		text-decoration: none;
		color: inherit;
	}
	.education {
		margin-top: 2rem;
		/* color: red; */
		margin-left: 1rem;
	}
	.experience {
		margin-top: 2rem;
		/* color: red; */
		margin-left: 1rem;
	}
	.relevant-skills {
		margin-top: 2rem;
		/* color: red; */
		margin-left: 1rem;
	}

	.experience-table th {
		padding-right: 250px;
	}

	.education-table th {
		padding-right: 260px;
	}

	.skills-table th {
		padding-right: 320px;
	}

	.top-div-for-decoration {
		margin-top: 20px;
		margin-bottom: 20px;
		padding-top: 20px;
		padding-bottom: 20px;
		background-color: cornflowerblue;
		color: cornflowerblue;
	}
	.hidden-text-in-top-div {
		display: none;
	}

	.white-box-in-middle-to-look-like-piece-of-paper {
		background-color: white;
		margin-left: 30px;
		padding-left: 25px;
		margin-right: 30px;
		padding-right: 25px;
		border: 1px black solid;
		height: 1000px;
	}
	.aside-front-page {
		margin-top: 1rem;
		margin-left: 1rem;
		width: 25%;
		/* color: hotpink; */
		border-right: 1px grey solid;
	}

	.objective-h2 {
		text-align: center;
	}
	.objective-p {
		padding: 12px;
	}
	.next-to-the-aside {
		/* display: inline-block; */
		width: 74%;
		text-align: left;
	}
	.container-for-everything {
		display: flex;
	}
</style>

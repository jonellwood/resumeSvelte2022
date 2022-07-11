<script>
	import Hr from '../lib/hr.svelte';
</script>

<div class="white-box-in-middle-to-look-like-piece-of-paper">
	<div class="top-div-for-decoration">
		<p class="hidden-text-in-top-div">
			IF YOU CAN SEE THIS TEXT YOU ARE PROBABLY VIEWING SOURCE. PLEASE FEEL FREE TO SUBMIT IDEAS TO
			MAKE THIS BETTER.
		</p>
	</div>
	<div class="certifications">
		<h1>Certifications / Courses Completed</h1>
		<table class="certifications-table">
			<tr>
				<th>Course / Certification</th>
				<th>Where</th>
				<!-- <th>Dates</th> -->
			</tr>
			<tr>
				<td>CompTIA CDIA+</td>
				<td />
				<!-- <td>December 2005</td> -->
			</tr>
			<tr>
				<td>CompTIA A+</td>
				<td />
				<!-- <td>June 2019</td> -->
			</tr>
			<tr>
				<td>W3C Certified Front End Web Developer</td>
				<td>Edx.org</td>
				<td />
			</tr>
			<tr>
				<td>Developing Cloud Applications with Node.js and React</td>
				<td>Edx.org</td>
				<td />
			</tr>
			<tr>
				<td>Intro to Computer Science and Programming Using Python</td>
				<td>Edx.org</td>
				<td />
			</tr>
			<tr>
				<td>JavaScript: From Fundamentals to Functional JS, v2</td>
				<td>Bianca Gandolfo, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>JavaScript: The Hard Parts, v2</td>
				<td>Will Sentence, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>JavaScript: The Recent Parts</td>
				<td>Kyle Simpson, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>JavaScript: The New Hard Parts</td>
				<td>Will Sentence, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Functional-Light JavaScript, v3</td>
				<td>Kyle Simpson, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Deep JavaScript Foundations</td>
				<td>Kyle Simpson, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Hardcore Functional Programming in JavaScript, v2</td>
				<td>Brian Lonsdorf, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Accessibility in JavaScript Applications</td>
				<td>Marcy Sutton, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Design for Developers</td>
				<td>Sarah Drasner, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>SVG Essentials & Animation, v2</td>
				<td>Sara Drasner, Frontend Master</td>
				<td />
			</tr>
			<tr>
				<td>Complete Into to React, v7</td>
				<td>Brian Holt, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Web Performance Fundamentals</td>
				<td>Todd Gardner, Frontend Masters</td>
				<td />
			</tr>
			<tr>
				<td>Beginner JavaScript</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
			<tr>
				<td>React for Beginners</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
			<tr>
				<td>ES6 for Everyone</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
			<tr>
				<td>Advanced React and GraphQL</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
			<tr>
				<td>Master Gatsby</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
			<tr>
				<td>CSS Grid</td>
				<td>Wes Bos, wesbos.com</td>
				<td />
			</tr>
		</table>
		<Hr />
	</div>
</div>

<style>
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
	.certifications {
		margin-top: 2rem;
		margin-left: 1rem;
	}
	.certifications-table th {
		padding-right: 350px;
	}
</style>

<template>
	<div class="container-fluid vh-65">
		<div class="d-flex align-items-start flex-column justify-content-center mx-5">
			<div class="header header-2 my-5">Experiences</div>
			<div class="container mt-4 bh3 fixed-width">
				<div class="d-flex align-items-start vertical">
					<div
						class="nav flex-column nav-pills me-3"
						id="v-pills-tab"
						role="tablist"
						aria-orientation="vertical"
					>
						<button
							class="nav-link nav-link-custom active"
							id="v-pills-home-tab"
							data-bs-toggle="pill"
							data-bs-target="#v-pills-home"
							type="button"
							role="tab"
							aria-controls="v-pills-home"
							aria-selected="true"
						>
							TCU
						</button>
						<button
							class="nav-link nav-link-custom"
							id="v-pills-profile-tab"
							data-bs-toggle="pill"
							data-bs-target="#v-pills-profile"
							type="button"
							role="tab"
							aria-controls="v-pills-profile"
							aria-selected="false"
						>
							TCU
						</button>
						<button
							class="nav-link nav-link-custom"
							id="v-pills-messages-tab"
							data-bs-toggle="pill"
							data-bs-target="#v-pills-messages"
							type="button"
							role="tab"
							aria-controls="v-pills-messages"
							aria-selected="false"
						>
							Freelance
						</button>
						<button
							class="nav-link nav-link-custom"
							id="v-pills-settings-tab"
							data-bs-toggle="pill"
							data-bs-target="#v-pills-settings"
							type="button"
							role="tab"
							aria-controls="v-pills-settings"
							aria-selected="false"
						>
							Start up
						</button>
					</div>
					<div class="tab-content" id="v-pills-tabContent">
						<div
							class="tab-pane fade show active"
							id="v-pills-home"
							role="tabpanel"
							aria-labelledby="v-pills-home-tab"
						>
							<h5 class="bh1 text-start">{{ job1des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job1Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job1" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade"
							id="v-pills-profile"
							role="tabpanel"
							aria-labelledby="v-pills-profile-tab"
						>
							<h5 class="bh1 text-start">{{ job2des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job2Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job2" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade"
							id="v-pills-messages"
							role="tabpanel"
							aria-labelledby="v-pills-messages-tab"
						>
							<h5 class="bh1 text-start">{{ job3des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job3Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job3" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade"
							id="v-pills-settings"
							role="tabpanel"
							aria-labelledby="v-pills-settings-tab"
						>
							<h5 class="bh1 text-start">{{ job4des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job4Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job4" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
					</div>
				</div>
				<!-- this is for horizontal -->
				<div class="horizontal">
					<nav class="horizontal-scroll">
						<div class="nav nav-pills my-3" id="nav-tab" role="tablist">
							<button
								class="nav-link active nav-link-custom-horizontal"
								id="nav-home-tab"
								data-bs-toggle="tab"
								data-bs-target="#nav-home"
								type="button"
								role="tab"
								aria-controls="nav-home"
								aria-selected="true"
							>
								TCU
							</button>
							<button
								class="nav-link nav-link-custom-horizontal"
								id="nav-profile-tab"
								data-bs-toggle="tab"
								data-bs-target="#nav-profile"
								type="button"
								role="tab"
								aria-controls="nav-profile"
								aria-selected="false"
							>
								TCU
							</button>
							<button
								class="nav-link nav-link-custom-horizontal"
								id="nav-contact-tab"
								data-bs-toggle="tab"
								data-bs-target="#nav-contact"
								type="button"
								role="tab"
								aria-controls="nav-contact"
								aria-selected="false"
							>
								Freelance
							</button>
							<button
								class="nav-link nav-link-custom-horizontal"
								id="nav-contact-tab"
								data-bs-toggle="tab"
								data-bs-target="#nav-contact"
								type="button"
								role="tab"
								aria-controls="nav-contact"
								aria-selected="false"
							>
								Start up
							</button>
						</div>
					</nav>

					<div class="tab-content" id="nav-tabContent">
						<div
							class="tab-pane fade show active mx-3"
							id="nav-home"
							role="tabpanel"
							aria-labelledby="nav-home-tab"
						>
							<h5 class="bh1 text-start">{{ job1des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job1Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job1" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade mx-3"
							id="nav-profile"
							role="tabpanel"
							aria-labelledby="nav-profile-tab"
						>
							<h5 class="bh1 text-start">{{ job2des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job2Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job2" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade mx-3"
							id="nav-contact"
							role="tabpanel"
							aria-labelledby="nav-contact-tab"
						>
							<h5 class="bh1 text-start">{{ job3des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job3Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job3" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
						<div
							class="tab-pane fade mx-3"
							id="nav-contact"
							role="tabpanel"
							aria-labelledby="nav-contact-tab"
						>
							<h5 class="bh1 text-start">{{ job4des }}</h5>
							<h6 class="bh5 mt-2 mb-3">{{ job4Time }}</h6>
							<h6 class="bh5 lh-base mx-3" v-for="(job, index) in job4" :key="index">
								<i class="fa fa-light fa-caret-right me-2" />
								{{ job }}
							</h6>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	export default {
		name: 'About',
		data() {
			return {
				job1des: 'Full-Stack Web Development Project',
				job1: [
					'Developed a Chinese Learning Platform system website/application project as part of my studies.',
					'Developed a full-stack application using Vue3 JS, SpringBoots, Auth0, MongoDB, Git.',
					'Utilized my skills in frontend and backend development, database management, and graphic design to build a user-friendly and visually appealing website/application.',
					'Designed and implemented features such as course management, student and teacher profiles, assignment submissions, and grades tracking.',
				],
				job1Time: 'Aug 2022 - Present',

				job2des: 'Java and Python-based system help desk',
				job2: [
					'Java and Python-based system help desk.',
					'Utilized knowledge of Java, Python, and MongoDB to troubleshoot and resolve a range of issues.',
					'Improving the program and student experience',
					'Provided guidance to students to improving the performance and user satisfaction.',
				],
				job2Time: 'Jan 2022 - May 2022',

				job3des: 'Freelance Web Developer',
				job3: [
					'Designed custom website for local nails salons. Increasing business traffic by almost 60%.',
					'Developed visually appealing and functional site that improved online visibility and customer engagement.',
					'Maintained and updated the website regularly to ensure smooth operation and address customer feedback',
				],
				job3Time: 'May 2018 - 2021',

				job4des: 'E-commerce Product Specialist',
				job4: [
					'Established an e-commerce platform to sell products online and conducted market research to identify customer needs and preferences.',
					'Facilitated the procurement of inventory and ensured customers had access to up-to-date delivery information',
				],
				job4Time: 'July 2018 - Aug 2019',
			};
		},
	};
</script>
<style>
	.horizontal {
		display: none;
	}
	.vh-65 {
		min-height: 60vh;
		height: auto;
	}
	.fixed-width {
		max-width: 750px;
	}
	h1 {
		color: var(--text-color1);
		font-size: 2rem;
	}
	.bh5 {
		color: var(--text-color2);
		text-align: left;
	}

	.header-2::before {
		content: '02.  ';
		left: 0;
		margin-right: 10px;
		font-size: 1.5rem;
		color: var(--primary-color);
	}

	/* active nav link */
	.nav-link-custom {
		color: var(--text-color1);
		text-align: left;
		padding: 5px 20px;
		border-left: 2px solid var(--decor-color) !important ;
		border-radius: 0 !important ;
		transition: border-left 0.5s ease-in-out;
		font-size: 0.9rem;
	}

	.nav-pills .nav-link-custom.active {
		background-color: var(--background-color) !important;
		color: var(--primary-color);
		border-left: 2px solid var(--primary-color) !important;
		border-radius: 0;
	}

	/* hover state */
	.nav-pills .nav-link-custom:hover {
		background-color: var(--background-color);
		color: var(--primary-color);
	}
	.nav-pills .nav-link-custom.active ~ .nav-link-custom {
		transition: border-left 0.5s ease-in-out;
	}

	.nav-pills .nav-link-custom.active ~ .nav-link-custom:hover {
		background-color: var(--background-color);
		color: var(--primary-color);
		border-left-color: var(--primary-color) !important;
	}
	/* For horizontal */

	.nav-link-custom-horizontal {
		color: var(--text-color1);
		text-align: left;
		padding: 5px 30px;
		border-bottom: 2px solid var(--decor-color) !important ;
		border-radius: 0 !important ;
		transition: border-left 0.5s ease-in-out;
		font-size: 0.9rem;
	}
	.nav-pills .nav-link-custom-horizontal.active {
		background-color: var(--background-color) !important;
		color: var(--primary-color);
		border-bottom: 2px solid var(--primary-color) !important;
		border-radius: 0;
	}

	.nav-pills .nav-link-custom-horizontal:hover {
		background-color: var(--background-color);
		color: var(--primary-color);
	}
	.nav-pills .nav-link-custom-horizontal.active ~ .nav-link-custom-horizontal {
		transition: border-left 0.5s ease-in-out;
	}

	.nav-pills .nav-link-custom-horizontal.active ~ .nav-link-custom-horizontal:hover {
		background-color: var(--background-color);
		color: var(--primary-color);
		border-bottom-color: var(--primary-color) !important;
	}

	.horizontal-scroll {
		overflow-x: auto;
	}
	.horizontal-scroll > .nav {
		flex-wrap: nowrap;
	}
</style>

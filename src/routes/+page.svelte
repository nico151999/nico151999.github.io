<script lang="ts">
	import LayoutGrid, { Cell } from '@smui/layout-grid';
	import { mdiAccount, mdiBriefcaseOutline, mdiSchool, mdiFlashOutline, mdiWeb } from '@mdi/js';
	import { Icon } from '@smui/common';
	import Card, { Content } from '@smui/card';
	import { Timeline, TimelineItem } from '@bonosoft/sveltekit-timeline';
	import { ImageAspectContainer, Image } from '@smui/image-list';
	import LinearProgress from '@smui/linear-progress';
</script>

<Cell span={12}>
	<h1>Nico Feulner</h1>
	<h2>DevOps & Software Engineer</h2>
</Cell>
<Cell spanDevices={{ phone: 12, tablet: 6, desktop: 6 }}>
	<Card>
		<Content>
			<h3>
				<Icon tag="svg" viewBox="0 0 24 24" style="height: 1.1em;">
					<path fill="currentColor" d={mdiAccount} />
				</Icon>
				Profile
			</h3>
			<LayoutGrid>
				<Cell spanDevices={{ phone: 12, tablet: 4, desktop: 4 }}>
					<ImageAspectContainer>
						<Image src="https://avatars.githubusercontent.com/u/10008855?v=4" alt="Image" />
					</ImageAspectContainer>
				</Cell>
				<Cell spanDevices={{ phone: 12, tablet: 8, desktop: 8 }}>
					<div style="text-align: justify; text-justify: inter-word;">
						<span
							>A DevOps engineer with a high proportion of Software Engineering tasks in his daily
							business. Has a passion for open source software, primarily the tools in the CNCF
							landscape and all things Kubernetes (declarative, distributed software❤️). Loves
							designing and implementing scalable software architectures and pipelines, and
							generally making complicated tasks easily and securely accessible. Likes to plan and
							develop highly-scalable, novel software solutions that reach and help a large number
							of people. Enjoys socializing as well as sharing and discussing technologies, findings
							and achievements both with colleagues and the community. Self-hosts everything the K8s
							way from his own music streaming service to smart home until everything crashes and he
							needs a flashlight to find the bathroom🔦.<br />
							Loves the outdoors with a passion for cycling🚲, hiking🥾 as well as skiing⛷ and is an
							active voluntary tour guide at DNT in Norway. Is into travelling🌎 and experiencing other
							cultures💬.
						</span>
					</div>
				</Cell>
			</LayoutGrid>
		</Content>
	</Card>
</Cell>
<Cell spanDevices={{ phone: 12, tablet: 6, desktop: 6 }}>
	<Card>
		<Content>
			<h3>
				<Icon tag="svg" viewBox="0 0 24 24" style="height: 1.1em;">
					<path fill="currentColor" d={mdiBriefcaseOutline} />
				</Icon>
				Work experience
			</h3>
			<Timeline>
				<TimelineItem status="ready">
					2024-present<br /><strong>DevOps Engineer</strong> (Conta AS, Ålesund)
					<ul>
						<li>
							Designing and building up a new infrastructure for the Norwegian market with GitOps
							based on Crossplane
						</li>
						<li>Developing and maintaining existing services further</li>
						<li>Maintaining and migrating old infrastructure to new one</li>
					</ul>
				</TimelineItem>
				<TimelineItem status="ready">
					2020-2024<br /><strong>DevOps Engineer</strong> (Deutsche Telekom IT GmbH, Bamberg)
					<ul>
						<li>
							Developed and operated an ordering, management and billing tool for a private
							Kubernetes platform based on Rancher (gRPC microservices written in Golang & Angular
							frontend)
						</li>
						<li>Built pipelines for testing and deploying software on Kubernetes</li>
						<li>
							Developed K8s controllers for automatic resource scalings in a GitOps-centric setup
						</li>
						<li>Led the software development tasks in this Kubernetes platform team</li>
						<li>
							Participated in building a GCP landingzone by integrating the user management in the
							internal IdP and building a project ordering tool
						</li>
					</ul>
				</TimelineItem>
				<TimelineItem status="ready">
					2017-2020<br /><strong>Dual Student in Applied Computer Science</strong> (Deutsche Telekom
					AG, Nuremberg/Bamberg)
					<ul>
						<li>
							Worked as an ordinary software engineer apart from few occassional course days at
							university
						</li>
						<li>Participated in an exchange programme at T-Systems Slovakia in Košice</li>
						<li>
							Contributed to a ticket system built with Symfony in a small team of Software
							Developers
						</li>
					</ul>
				</TimelineItem>
			</Timeline>
		</Content>
	</Card>
</Cell>
<Cell spanDevices={{ phone: 12, tablet: 6, desktop: 6 }}>
	<Card>
		<Content>
			<h3>
				<Icon tag="svg" viewBox="0 0 24 24" style="height: 1.1em;">
					<path fill="currentColor" d={mdiSchool} />
				</Icon>
				Education
			</h3>
			<Timeline>
				<TimelineItem status="ready">
					2021-2023<br /><strong>MSc Computer Science with Artificial Intelligence</strong> (University
					of York)
				</TimelineItem>
				<TimelineItem status="ready">
					2017-2020<br /><strong>BSc Applied Computer Science</strong> (Hochschule für Telekommunikation
					Leipzig)
				</TimelineItem>
			</Timeline>
		</Content>
	</Card>
</Cell>
<Cell spanDevices={{ phone: 12, tablet: 6, desktop: 6 }}>
	<Card>
		<Content>
			<h3>
				<Icon tag="svg" viewBox="0 0 24 24" style="height: 1.1em;">
					<path fill="currentColor" d={mdiFlashOutline} />
				</Icon>
				Skills
			</h3>
			<ul>
				<li>
					<strong>Cloud technologies</strong><br />
					has broad experience working with both public and private clouds as well as employing a wide
					range of cloud-native products and maintaining the infrastructure declaratively. Simply loves
					doing things the K8s way both privately and at work.
				</li>
				<li>
					<strong>Programming</strong><br />
					writes software (mostly microservices, frontends and K8s operators but has experience with
					a wider range of technologies, e.g. Android) at scale in various languages and frameworks (lately
					mostly Golang and Java with Micronaut but has professionally worked with many other frameworks
					before)
				</li>
				<li>
					<strong>CI/CD</strong><br />
					has lots of experience working with modern CI/CD tooling, first and foremost Gitlab Pipelines,
					Github Actions and GitOps tools like ArgoCD and Flux
				</li>
				<li>
					<strong>Testing</strong><br />
					is experienced using several testing concepts and frameworks effectively (knows how to write
					them well and not only for high code coverage scores)
				</li>
				<li>
					<strong>Agile work</strong><br />
					has experience working both in custom collaboration environments and in common agile team collaboration
					frameworks (e.g. Scrum, SAFE) with related tooling
				</li>
			</ul>
		</Content>
	</Card>
</Cell>
<Cell spanDevices={{ phone: 12, tablet: 6, desktop: 6 }}>
	<Card>
		<Content>
			<h3>
				<Icon tag="svg" viewBox="0 0 24 24" style="height: 1.1em;">
					<path fill="currentColor" d={mdiWeb} />
				</Icon>
				Languages
			</h3>
			<ul>
				<li>
					<strong>German</strong><br />
					Mother tongue
					<LinearProgress progress={1} />
				</li>
				<br />
				<li>
					<strong>English</strong><br />
					Fluent
					<LinearProgress progress={0.9} />
				</li>
				<br />
				<li>
					<strong>Norwegian</strong><br />
					Advanced
					<LinearProgress progress={0.8} />
				</li>
				<br />
				<li>
					<strong>Latin</strong><br />
					Basic
					<LinearProgress progress={0.4} />
				</li>
			</ul>
		</Content>
	</Card>
</Cell>

<style>
	h1 {
		font-size: 3em;
		text-align: center;
	}

	h2 {
		font-size: 2em;
		text-align: center;
	}

	h3 {
		display: flex;
		align-items: center;
	}
</style>

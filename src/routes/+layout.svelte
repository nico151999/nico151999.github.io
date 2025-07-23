<script lang="ts">
	import TopAppBar, { Row, Section } from '@smui/top-app-bar';
	import Tooltip, { Wrapper } from '@smui/tooltip';
	import { mdiEmail } from '@mdi/js';
	import LayoutGrid from '@smui/layout-grid';
	import IconButton, { Icon } from '@smui/icon-button';
	import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
	import { faGithub } from '@fortawesome/free-brands-svg-icons';
	import '../app.scss';

	const email = 'nico.feulner@gmail.com';

	const openGithubProfile = () => {
		window.open('https://github.com/nico151999', '_blank');
	};

	const sendEmail = () => {
		window.open(`mailto:${email}`, '_self');
	};
</script>

<header>
	<TopAppBar variant="static" prominent={false} dense={true} color="primary">
		<Row>
			<Section align="end" toolbar>
				<Wrapper>
					<IconButton class="material-icons" aria-label="Email" onclick={sendEmail}>
						<Icon tag="svg" viewBox="0 0 24 24">
							<path fill="currentColor" d={mdiEmail} />
						</Icon>
					</IconButton>
					<Tooltip>{email}</Tooltip>
				</Wrapper>
				<IconButton onclick={openGithubProfile}>
					<FontAwesomeIcon icon={faGithub} />
				</IconButton>
			</Section>
		</Row>
	</TopAppBar>
</header>
<main>
	<LayoutGrid>
		<slot />
	</LayoutGrid>
</main>

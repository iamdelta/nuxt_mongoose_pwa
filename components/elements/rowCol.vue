<template>
	<v-row :justify="center ? 'center' : null">
		<v-col
			:class="textCenter ? 'text-center' : null"
			:sm="condense ? 8 : null"
			:lg="condense ? 6 : null"
			:xl="condense ? 4 : null"
		>
			<slot />
		</v-col>
	</v-row>
</template>

<script lang="coffee">

	export default

		props:
			center:
				type: Boolean
				default: true
			textCenter:
				type: Boolean
				default: true
			condense:
				type: Boolean
				default: false

</script>
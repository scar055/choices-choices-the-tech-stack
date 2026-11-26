<template>
	<section>
		<form>
			<List />
			<List />
			<List />
			<List />
			<List />
			<List />
			<List />
			<button>send</button>
		</form>
	</section>
</template>

<style>
:root {
	/* Primary blue colors */
	--blue-700: hsl(203, 90%, 22%);
	--blue-600: hsl(203, 85%, 32%);
	--blue-500: hsl(203, 80%, 42%);
	--blue-500-ring: hsl(203 80% 42% / 20%);
	--blue-400: hsl(203, 75%, 52%);
	--blue-300: hsl(203, 65%, 65%);
	--blue-200: hsl(203, 60%, 78%);
	--blue-100: hsl(203, 55%, 90%);
	--blue-50: hsl(203, 50%, 95%);

	/* Secondary red / alert */
	--red-700: hsl(4, 75%, 25%);
	--red-600: hsl(4, 70%, 35%);
	--red-500: hsl(4, 65%, 45%);
	--red-400: hsl(4, 60%, 55%);
	--red-300: hsl(4, 55%, 65%);
	--red-200: hsl(4, 50%, 75%);
	--red-100: hsl(4, 45%, 85%);

	/* Accent orange */
	--orange-700: hsl(30, 80%, 28%);
	--orange-600: hsl(30, 75%, 38%);
	--orange-500: hsl(30, 70%, 48%);
	--orange-400: hsl(30, 65%, 58%);
	--orange-300: hsl(30, 60%, 68%);
	--orange-200: hsl(30, 55%, 78%);
	--orange-100: hsl(30, 50%, 88%);

	/* Accent green */
	--green-700: hsl(150, 90%, 18%);
	--green-600: hsl(150, 85%, 28%);
	--green-500: hsl(150, 80%, 38%);
	--green-400: hsl(150, 75%, 48%);
	--green-300: hsl(150, 65%, 60%);
	--green-200: hsl(150, 55%, 72%);
	--green-100: hsl(150, 45%, 85%);

	/* Group theme colors */
	--theme-charcot: #ae4bbd;
	--theme-classification: #e8b809;
	--theme-infection: #8db331;
	--theme-prevention: #e6762c;
	--theme-pad: #028d8f;
	--theme-offloading: #009bcb;
	--theme-wound-healing: #6a77dd;

	/* Neutral / grey */
	--grey-900: hsl(210, 14%, 9%);
	--grey-700: hsl(210, 12%, 15%);
	--grey-600: hsl(210, 10%, 25%);
	--grey-500: hsl(210, 8%, 40%);
	--grey-400: hsl(210, 7%, 55%);
	--grey-300: hsl(210, 6%, 70%);
	--grey-200: hsl(210, 5%, 80%);
	--grey-100: hsl(240, 4%, 95%);
	--grey-50: hsl(210, 5%, 98%);

	/* Backgrounds */
	--background-color-primary: hsl(0, 0%, 100%);
	--background-color-secondary: hsl(210, 10%, 97%);

	/* Text */
	--main-text-color: var(--grey-700);
	--font-color-card: hsl(0, 0%, 26%);

	/* Notification */
	--favorite-notification-color: hsl(54, 100%, 60%);

	/* Box Shadows */
	--shadow-sm: 0 0.125rem 0.25rem hsla(213, 12%, 15%, 0.08);
	--shadow-md:
		0 0.25rem 0.75rem hsla(0, 12%, 15%, 0.12),
		0 0.125rem 0.25rem hsla(213, 12%, 15%, 0.08);
	--shadow-lg:
		0 0.5rem 1rem hsla(213, 12%, 15%, 0.15),
		0 0.25rem 0.5rem hsla(213, 12%, 15%, 0.1);
}

fieldset {
	border: none;
	padding: 0;
	margin: 0;

	display: flex;
	flex-direction: column;
	gap: 1rem;
	background-color: var(--grey-100);
	padding: 1rem;
	border-radius: 1rem;
}

legend {
	color: var(--blue-700);
	font-weight: 400;
	background-color: var(--blue-100);
	padding: 0.6rem;
	border-radius: 1rem;
}

label {
	display: flex;
	flex-direction: row;
	gap: 0.5rem;
	color: var(--blue-700);
	cursor: pointer;
	padding-left: 0.5rem;
	padding: 0.5rem;
}

label:hover {
	color: var(--main-text-color-light);
	border-radius: 1rem;
	background-color: var(--grey-200);
	padding: 0.5rem;
}

input[type="radio"] {
	accent-color: var(--orange-700);
	height: 15px;
	width: 15px;
	display: flex;
	flex-direction: row;
	justify-content: center;
}

label:has(input[type="radio"]:checked) {
	color: var(--main-text-color-light);
	border-radius: 1rem;
	background-color: var(--orange-400);
	padding: 0.5rem;
}
</style>

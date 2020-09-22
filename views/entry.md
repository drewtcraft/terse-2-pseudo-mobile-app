# Entry
The main view of the app.

## Layout
- A <select> style element for sorting with the options "newest" and "oldest" on the top of the page.  
- A list of episodes as full-width cards

## On View Load
1. Request a manifest at /manifest/[newest|oldest]/{page}
2. Render the manifest as a list of episodes

## Interactivity
- When the sort selection element is changed, the view should request a new manifest with page=0 and re-render.
- When an episode is clicked:
	1. Request all of the assets listed in the manifest, including the episode.json file and all of the images. 
	2. Track the loading progress of each image and display it on a loading indicator somewhere.
	3. Once all the images are loaded, pass all data into the episode view and change views.



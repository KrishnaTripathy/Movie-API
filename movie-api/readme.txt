TVMAZE WEBSITE YOU HAVE TO TAKE API
url : https://api.tvmaze.com/search/shows?q=girls

function makeImages(movies) {
    // Define a function named 'makeImages' that takes a single parameter 'movies'.
    for (let movie of movies) {
        // Iterate over each 'movie' in the 'movies' array using a for-of loop.
        let src = movie.show.image.medium;
        // Extract the image URL from the 'medium' property of the 'image' object
        // within the 'show' object of the current 'movie'.

        const img = document.createElement('img');
        // Create a new 'img' element.

        img.src = src;
        // Set the 'src' attribute of the 'img' element to the extracted image URL.

        container.appendChild(img);
        // Append the 'img' element to the 'container' element in the DOM.
    }
}

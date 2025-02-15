# Project 1 - Flixter

**Name of your app** shows the latest movies currently playing in theaters. The app utilizes the Movie Database API to display images and basic information about these movies to the user.

Time spent: **10** hours spent in total

## User Stories

The following **required** functionality is completed:

* [X] User can **scroll through current movies** from the Movie Database API
* [X] Display a nice default [placeholder graphic](https://guides.codepath.org/android/Displaying-Images-with-the-Glide-Library#advanced-usage) for each image during loading
* [X] For each movie displayed, user can see the following details:
  * [ X Title, Poster Image, Overview (Portrait mode)
  * [X] Title, Backdrop Image, Overview (Landscape mode)
* [X] Allow user to view details of the movie including ratings within a separate activity

The following **stretch** features are implemented:

* [X] Improved the user interface by experimenting with styling and coloring.
* [X] Apply rounded corners for the poster or background images using [Glide transformations](https://guides.codepath.org/android/Displaying-Images-with-the-Glide-Library#transformations)
* [X] Apply the popular [View Binding annotation library](http://guides.codepath.org/android/Reducing-View-Boilerplate-with-ViewBinding) to reduce boilerplate code.
* [X] Allow video trailers to be played in full-screen using the YouTubePlayerView from the details screen.

The following **additional** features are implemented:

* [X] Scrolling
* [X] Dark mode (background color, text color)
* [X] Fonts

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src="./vert.gif" title='Video Walkthrough' width=300 alt='Video Walkthrough' />
<img src="./horiz.gif" title='Video Walkthrough' width=600 alt='Video Walkthrough' />

GIF created with [Kap](https://getkap.co/).

## Notes
Challenges encountered during the creation of my app include:

Solved
1. No orientation rotation - I thought there was an issue with my code but the autorotate was not enabled on by default my emulator.
2. Movie list not showing up - I wasn't able to get to my breakpoints or see any of the messages logged after sending the API request to retrieve the movie information. After researching the issue, I saw that the issue was because of a memory shortage in my emulator so I was able to solve the issue by performing a cold boot on my emulator.

In Progress
1. Showing image on the Movie Details activity using Gradle - I tried creating a new class that extended GradleModule in order to show the image. However, I ran into mutliple issues and did not have time to complete this.
2. Trying to figure out how to use ViewBinding for Adapters (for RecyclerView)

## Open-source libraries used

- [Android Async HTTP](https://github.com/loopj/android-async-http) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Android

## License

    Copyright [2022] [Serena Zeng]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

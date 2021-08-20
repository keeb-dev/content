This weekend I want to see what Network Traffic I can see using existing [Kentik Labs](https://kentiklabs.com) related to VPC networks on DigitalOcean.

I like these types of projects because it puts an onus on creating a complicated test harness and I can end up building a bunch of toys to realize the vision. That there's a springboard for other other stuff to play around with is a side benefit.

## What to do?

* Set up distributed architecture - ui, api, and storage with simple nodes
* Make simple webapp - store/retrieve photos
* Make api for random photo
* Make website that displays a random photo in pool
* Make simple load testing script which uses random photo website
* Of course, make this easily deployable / repeatable

## What I want to end up showing?

Just getting one of these up and working is going to create enough

* Look out for normal flow, in/out_bytes for normal course
* Traffic spike!! Saturate link
* API service is broken
* Storage service is broken
* All of this is over `known ports` - flag any traffic on *unknown* ports
* All of this traffic should be `internal` - flag any traffic that is not

## Why photos?

Meaningful traffic, really. If it's simple HTTP requests of text the graphs aren't going to be as pronounced, either in traffic spikes or traffic dips

## Making it real, take some risks in the name of science

One of the side effects here is what happens if you make a thin UI/API layer that is backed by a free/cheap distributed storage provider like StorJ. Are there people out there looking for a place to store and share photos with a simple UI that is easily embeddable (like imgur used to be?)

How long will it take to get 1 user? 10 users? What's the geography of the people/ip accessing? How soon will it be taken over by nefarious people and will be forced to shut down?


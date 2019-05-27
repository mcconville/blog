---
layout: post
category : anton
tagline: "Supporting tagline"
tags : [technology]
---

Thought I'd jot down a few notes about reflections and observations of [KubeCon Europe 2019](https://events.linuxfoundation.org/events/kubecon-cloudnativecon-europe-2019/).

<img src="https://raw.githubusercontent.com/mcconville/blog/gh-pages/images/kubeconeu2019%402x.png" width="100%">

I didn't attend as many sessions as I'd like - about half my time at the conference was spent either preparing to speak at the IBM mini theatre, speak at the mini theatre or help at the booth - there to work ... so these are thoughts about the few sessions I was able to attend ...

[Mental Health in Tech - Dr Jennifer Akullian](https://kccnceu19.sched.com/event/NyYU/mental-health-in-tech-dr-jennifer-akullian-growth-coaching-institute)

Was happily surprised to see this on the agenda of Cloud Tech conference. I've been managing a development team for almost two years now, and try to be conscious of the human challenges, as well as the work challenges we face - so I welcome any insight into the subject of mental health in technology.

Jennifer recounted a few personal stories and perspectives. She shared some eye opening statistics about the rates and weights of mental health challenges in the tech workplace, and gave a few pointers of advice.

Definitely a talk to watch again when the videos are posted.

[Strategies to 'Kubernetify' Legacy Applications - Sai Vennam](https://kccnceu19.sched.com/event/MPXo/strategies-to-kubernetify-legacy-applications-sai-vennam-ibm)

Sai is an IBM colleague - I've been lucky to collaborate with him on a couple of projects. In this talk he sped through a few examples from 'lift and shift' to extending a classic Java application to Kube. It was very well done, with a slick performance from Sai - he certainly has a gift for this :)

The hall was large and packed - which gives a clue that the developer world has an appetite for this subject. One of my own talks was about app modernization, and I detected a similar hunger from my much smaller crowd about approaches and case studies.

Would recommend Sai's video when it is posted.

[Testing Your K8s Apps with Kind - Benjamin Elder & James Munnely](https://kccnceu19.sched.com/event/MPYy/testing-your-k8s-apps-with-kind-benjamin-elder-google-james-munnelly-jetstackio)

A minimal, but very informative presentation about unit and integration testing of Kube apps. [Kind](https://github.com/kubernetes-sigs/kind) is a fast, lightweight, cross platform and 'hermetic' tool for running tests.

Another good talk - clear, concise, and useful. Impressive.

[Chaos Debugging - Idit Levine & Mitch Kelley](https://kccnceu19.sched.com/event/MPXi/chaos-debugging-finding-and-fixing-microservice-weak-points-idit-levine-mitch-kelley-soloio)

Began with the funny because true observation that [we replaced our monolith with micro services so that every outage could be more like a murder mystery.](https://twitter.com/honest_update/status/651897353889259520?lang=en)

They shared a few tools to debug in real time, which if they can be set up as easily as they claim, look super useful and fun to work with ...

[Squash](https://squash.solo.io/) for real time Debugging

Another called ServiceMesh? which is not open source yet, but which allows requests to be recorded.

And another called [Gloo](https://gloo.solo.io) which I have to admit my brain was already too overwhelmed and impressed by Squash to tune into. It was a jam packed but very decent presentation. Would recommend a view when posted.

[Building Cross Cloud ML Pipelines - Holden Karau & Trevor Grant](https://kccnceu19.sched.com/event/MPaZ/building-cross-cloud-ml-pipelines-with-kubeflow-with-spark-tensorflow-holden-karau-google-trevor-grant-ibm)

The presenters shared a link for a [forthcoming book](http://www.introductiontomlwithkubeflow.com/)

I'm really interested in machine learning, and regret not having more time to really immerse in it. I was hopeful that this talk was going to be a practical walkthrough, but it was a somewhat jovial, and anecdotal list of steps, I felt for people a bit more clued into the topic. So I was somewhat disappointed by this talk.

[Building Cloud Native GDPR Friendly Systems - Zsolt Homorodi](https://kccnceu19.sched.com/event/MPYC/building-cloud-native-gdpr-friendly-systems-for-data-collection-zsolt-homorodi-vtt)

I got a lot out of this talk. I'm usually not a one for bullet pointed slides, but with such a nebulous topic of GDPR, I felt that they really worked this time, to introduce the relevance and challenges for developers.

The talk was in a couple of parts - the first part introduced the reasons to care, and the operational boundaries of gathering data. This part alone makes a great presentation ...

... which was good, because the second part was a demo that ran over the allotted time - it was the presenter's first conference, and I don't fault him for this, since it was generally a super useful and inspiring talk for me.

The presenter works at a government sponsored research organization in Finland - where they work hard to protect privacy and adhere to the rules. He mentioned that throughout Europe, during the first 9 months of GDPR approximately 50 million Euros in fines had been issued, with over 200,000 complaints of violations.

I found [this site tracking some of the cases](https://alpin.io/blog/gdpr-fines-list/)

I'm especially interested in this for some upcoming work, and think it makes a really fascinating and important topic for the future of cloud tech. Definitely a talk to look out for when posted.

-

In general I found the conference well organized, in an enormous venue. For me personally it was the second half of a long business trip to Europe ... I was jaded in the the evenings from preparing my own three talks, or/and working my shifts at the booth ... and then immersing in other people's talks, so I regret not being more sociable this time around. I really wanted to get the most out of the work time I had there.

I was staying at a hotel closer to the city, so it took me 30 minutes on the train each day ... and prepping for a half marathon the day after I returned to Canada ... so distracted a bit.

Otherwise, I really valued the conversations at the booth, and the observations about my own projects ( which I'll share more about in the coming months ). And I got a lot from these talks. Thanks to all who made it possible for me to travel, and for all of those who shared time and information with me :)

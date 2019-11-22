---
layout: post
category : anton
tagline: "Supporting tagline"
tags : [technology]
---

Writing this from San Diego, at the end of another intense KubeCon conference. I was here as part of IBM's staff, to present a couple of sessions at the mini theatre, and to take a shift at the IBM booth, but when not taking my turn at the booth, I attended as many talks as I could. Here are my notes ...

<img src="https://raw.githubusercontent.com/mcconville/blog/gh-pages/images/kubeconna%402x.png" width="100%">

General themes - use of service ServiceMesh ( mostly Envoy from the talks I was able to attend ), economics of cloud services, and machine learning - both in terms of devops, and in terms of building ML on Kube.

[Measuring and optimizing ML Workloads at Lyft](https://events19.linuxfoundation.org/events/kubecon-cloudnativecon-north-america-2019/schedule/)

The first talk I attended, and I think the most inspiring one that I attended ... definitely has me thinking about a lot of different things.

The essence of the session was about how at Lyft they've begun using Machine Learning to understand their infrastructure bill better. They build on AWS. Estimating, and justifying cloud usage fascinates me. From this talk I feel we're still at the finding a way of accounting, and navigating the economics of cloud computing.

Themes that stood out to me - attribution schedules, allocation of resources, versus efficiency of use. Different workloads have different needs, at different times.

Aside from the content of the talk, the presenter was outstanding - although just a recent hire, his clarity of communication, and depth of understanding of this topic was super impressive.

[How Spotify Migrated Ingress HTTP Systems to Envoy](https://events19.linuxfoundation.org/events/kubecon-cloudnativecon-north-america-2019/schedule/)

There seemed a lot of talks about Envoy this conference. I'm personally still trying to understand the [differences/similarities between Envoy and Istio](https://stackshare.io/stackups/envoy-vs-istio)

I loved hearing these insights from some of the companies that serve millions of users ...

Spotify serve 8 million requests per second. Their system serves 79 markets, 248 million monthly users and is built on 1200 microservices - almost all on Google Cloud.

This was a well delivered talk that walked through the problems they were attempting to solve, why they chose Envoy to solve them.

Before switching to Envoy, they felt their old gateway Was

- underinvested
- had service discovery headaches
- had high operational conversations

With Envoy ...

- a cloud native perimeter
- vibrant community
- service discovery

They implemented and moved in a way where product teams needed to understand as little as possible about the switch. They built gradually, with minimum disruption to their dev teams and end users. They facilitated a quick fallback in case of problems.


[Moving from Legacy Infrastructure to the Cloud in a Government Organization - Chris Carty, City Of Ottawa](https://events19.linuxfoundation.org/events/kubecon-cloudnativecon-north-america-2019/schedule/)

Happy coincidence for me that a senior engineer from my own city's municipal government was presenting their story of evolution to the cloud.

He did our city proud, with his talk too - very well presented and organized story - a checklist of considerations for any government or any organization in moving from mainframe based solutions to kubernetes.

In Ottawa's case the city employees 17,000 people, has 120 lines of business ad 400 apps to support ( Java, DotNET and Perl ). Some of the mainframes are end of life, and rather than renew them, they've begun migrating solutions to Microsoft Azure.

I recommend watching his talk, or asking for his slides - he has really beaten a path for others to follow if they're embarking on a similar journey.

One point of interest for me, and I raised a laugh in asking, tongue in cheek ... was what this means for me as a tax payer. I am curious about how they evaluate costs ... so they are no longer paying for mainframes, but does that mean they work with the same budget for cloud resources? Have they modeled or estimated their use. Is this a net savings, or a net add? The presenter said they were not there yet - in estimating or projecting.

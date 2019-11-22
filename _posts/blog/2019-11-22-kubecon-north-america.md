---
layout: post
category : anton
tagline: "Supporting tagline"
tags : [technology]
---

Writing this from San Diego, at the end of another intense KubeCon conference. I was here as part of IBM's staff, to present a couple of sessions at the mini theatre, and to take a shift at the IBM booth, but when not taking my turn at the booth, I attended as many talks as I could. Here are my notes ...

<img src="https://raw.githubusercontent.com/mcconville/blog/gh-pages/images/kubeconna%402x.png" width="100%">

General themes - use of service ServiceMesh ( mostly Envoy from the talks I was able to attend ), economics of cloud services, and machine learning - both in terms of devops, and in terms of building ML on Kube.

[Measuring and optimizing ML Workloads at Lyft](https://sched.co/UabJ)

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


[Moving from Legacy Infrastructure to the Cloud in a Government Organization - Chris Carty, City Of Ottawa](https://sched.co/UabP)

Happy coincidence for me that a senior engineer from my own city's municipal government was presenting their story of evolution to the cloud.

He did our city proud, with his talk too - very well presented and organized story - a checklist of considerations for any government or any organization in moving from mainframe based solutions to kubernetes.

In Ottawa's case the city employees 17,000 people, has 120 lines of business ad 400 apps to support ( Java, DotNET and Perl ). Some of the mainframes are end of life, and rather than renew them, they've begun migrating solutions to Microsoft Azure.

I recommend watching his talk, or asking for his slides - he has really beaten a path for others to follow if they're embarking on a similar journey.

One point of interest for me, and I raised a laugh in asking, tongue in cheek ... was what this means for me as a tax payer. I am curious about how they evaluate costs ... so they are no longer paying for mainframes, but does that mean they work with the same budget for cloud resources? Have they modeled or estimated their use. Is this a net savings, or a net add? The presenter said they were not there yet - in estimating or projecting.

[Flyte: Cloud Native Machine Learning & Data Processing Platform - Ketan Umare & Haytham AbuelFutuh, Lyft
](https://sched.co/UaYY)

I'd heard about [Flyte](https://lyft.github.io/flyte/index.html) and wanted a bit more insight.

Lyft wanted a way to build reliable, scaleable, reproducable models ... especially when it came to reporting on business results internally every quarter. They had lost a key data scientist who had a lot of intellectual property on their own laptop, and had been the only data scientist using it at the time.

This talk was a walkthrough. I am super interested in machine learning, and really want to get into it, but have far too many interests, and now that I'm managing a team, still creating case studies, and still learning more about the cloud, I need to be selective about where I invest my time and how. I'm not sure Flyte is my entry point ... I want to learn more about the basics of tensorflow and models. However, I think this is a good overview if yoy want to learn more check out the video when it is up.


[How Yelp Moved Security From the App to the Mesh with Envoy and OPA - Daniel Popescu, Yelp & Ben Plotnick, Cruise](https://sched.co/UaZT)

A really well presented talk about Yelp's adoption of a service mesh to improve security of their apps. Really well presented :)

Takeaways - moving from a 15 year old monolith to microservices for authentication and authorization. Respecting developers who would consume Yelp through integrations - always considering the restful service pains they would need to suffer with any architectural decisions they made.

Again Yelp adopted Envoy in their solution for this. Although one of the engineers began the talk by wishing that Istio existed before they started their migration of services. I wanted to ask why he would have preferred that. Maybe I'll send a message to him.

Things to look up from this talk: [Open Policy Agent](https://www.openpolicyagent.org/)

Executive notes:

- Security in service mesh makes Yelp services secure by default
- Work incrementally ( same approach as talk above from Spotify )
- Automate migrations
- The use case is the north started

[Security Beyond Buzzwords: How to Secure Kubernetes with Empathy? - Pushkar Joglekar, Visa](https://sched.co/Uad6)

Another wonderful talk - I loved how well organized the presentation was. He based it around an acronym of security considerations - a [threat model](https://dev.to/petermbenjamin/demystifying-stride-threat-models-230m)

Spoof
Tamper
Repudiation
Information Disclosure
DOS
Elevation of Privileges

Where he explored what each of those meant for Kubernetes and encouraged an exploration of them as a graph.

I kind of want to follow this idea for GDPR.

Great talk.

[Tutorial: From Notebook to Kubeflow Pipelines: An End-to-End Data Science Workflow](https://sched.co/Uaeq)

This was a very slick 90 minute tutorial from Google ... the most impressive part for me was how well executed it was, in setting up Kube resources, installing Kubeflow, the data model etc.

It introduced a tool called [Kale](https://github.com/kubeflow-kale) which attempts to simplify kubeflow pipelines.

It all worked well, I was able to get to the end of the tutorial - deploy a pipeline, work through the sample data ... but it isn't what I really want, which is to understand tensorflow and work from first principles with my own data.

I need to do that work myself. Otherwise - impressive tutorial and technology :)

[Fine Grained Mesh Metrics for Better Visibility With Native Performance - Mandar Jog & Kuat Yessenov, Google](https://sched.co/UaYV)

This session served to open my eyes to the idea of mesh metrics rather than educate me about a specific implementation - mostly because my brain was getting kind fried this late in the week, and after the kubeflow tutorial earlier in the day.

All in all, I feel inspired to learn more about mesh, build more examples with it, and personally to dig into tensorflow/kubeflow in 2020. I also have a swath of ideas about exploring the economics of cloud usage - have discussed with a colleague to collaborate with in 2020 too.

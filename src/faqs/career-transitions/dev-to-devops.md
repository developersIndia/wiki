<!-- omit from toc -->

# Developer to DevOps

- [Perspectives \& advice from the Community](#perspectives--advice-from-the-community)
- [Stories from the community](#stories-from-the-community)

## Perspectives & advice from the Community

`u/reophos` on a post titled
[How to switch from Developer role to DevOps role? I am highly fascinated by DevOps roles, don't know why?](https://www.reddit.com/r/developersIndia/comments/1b585la/how_to_switch_from_developer_role_to_devops_role/)
shared the following advice:

<blockquote>

Since many here have already covered the negative aspects of the role if you
join in an organisation that does not implement DevOps properly. I will share
the positive aspects. I have 3.5 YOE as DevOps.

The original idea to implement DevOps was so to bridge the difference between
Developers and Operations. How can Operations manage an application effectively
when they've not built it? Developers should spend some time doing operations
for the applications they're building, so they can better manage outages, do
RCAs faster, do their own deployments. In my perspective, a team is doing DevOps
properly if their Devs are responsible for their code in production and getting
into production.

So, why do organisations hire 'DevOps' Engineers even when their Developers can
do the above? Because the developers can do it, but there is an abstraction,
they generally don't understand the whys and hows of the processes, and the
operations work they do is limited to their applications. In my org, Devs write
their own Terraform for the AWS infra they need - lambdas, ECRs, API Gateway
etc. We put the process in place and validate this. But as a DevOps person your
work is not limited at all.

People say things get boring after the build processes are in place. I don't
think they're working in orgs that implement DevOps properly. We're a B2B
startup in the Gaming Industry. In the last few months, we've been having the
time of our lives, working on load testing our serverless infrastructure finding
bottlenecks as we are anticipating a huge load with a new big customer acquired.
Found some very interesting bugs and I even went ahead and fixed it, so the
onboarding went smoothly. Reduced build times greatly for the developers by
introducing remote caching for their lambda docker image builds, and
implementing Terraform module caching. Learnt a lot about Postgres locks,
indexes, and partitions as we are now handling billions of data and don't want
any queries to be deplayed because of the databse. Did database migrations
between different AWS RDS Servers. And these are all just the tip of the iceberg
as we scale.

We do a little bit of development work as well from time to time, wrote an API
to sync user informations between the Identity Provider and DB. As part of the
engineering team, we are also responsible to be actively in the know of product
and give feedback.

We are responsible to implement so many new things, and keep guardrails. It is
all the fun!

It also has to do a lot with the attitude of the team as well. We do blameless
RCA. When something goes wrong, find why the process failed you there and fix
that instead of blaming the person. We face incidents, but I don't think any of
us fear about it. I am excited to see what process can be improved.

So, coming to your questions, best possible way to switch is probably getting to
switch internally first and then go for other orgs. It will be hard to get a
role without experience and seeing you are 3 YOE, I don't think you want to
start from 0 again. Other ways is to get familiar with DevOps stuff in your free
time and showcase your skill in GitHub, as blogs, in LinkedIn etc. Set up a home
lab. Do some self-hosted stuff. Learn cloud, K8s, Terraform. And number of roles
are generally limited in product orgs. So, getting an interview might be harder
than your standard dev role as you said. When you do get the interview, ask them
questions about the processes and the way they do deployments, RCA to understand
their work culture. Decide if you want to join them.

Coming to DevOps from Dev is a great plus, only if you were a developer, you'll
understand the pain points of these processes truly, you can streamline them a
lot easier.

---

[`Source`](https://www.reddit.com/r/developersIndia/comments/1b585la/comment/kt4eg25/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)

</blockquote>

`@spookyintheam` on developersIndia Discord (#devops channel) shared the
following **resources to get started with DevOps**:

<blockquote>

I see there are no resources in this channel related to DevOps so I guess I'll
my own resources that I've used over the years.

- Roadmap itself: [https://roadmap.sh/devops](https://roadmap.sh/devops).
- [github.com/MichaelCade/90DaysOfDevOps](https://github.com/MichaelCade/90DaysOfDevOps),
  this is a pretty nice repository if you want to learn about the various tools
  and stuff that's used in a normal DevOps engineer's everyday life.
- For languages: I say Python and Go are the best languages for this field since
  you can code as well as write scripts.
  - Here's a roadmap for Go dev:
    [https://roadmap.sh/golang](https://roadmap.sh/golang).
  - And this playlist by Hitesh is good intro to the programming language:
    [Let's go with golang](https://www.youtube.com/playlist?list=PLRAV69dS1uWQGDQoBYMZWKjzuhCaOnBpa).
  - And this site for practising Go:
    [https://gophercises.com/](https://gophercises.com/).
- I don't know any resource for this since I learnt it over the years but master
  Linux and bash scripting
- Docker:
  - [Docker Tutorial for Beginners [FULL COURSE in 3 Hours]](https://www.youtube.com/watch?v=3c-iBn73dDE)
    this video by Nana is pretty good introduction to using Docker.
- Kubernetes:
  - [https://www.youtube.com/watch?v=X48VuDVv0do](https://www.youtube.com/watch?v=X48VuDVv0do)
    by the same creator. Its a bit dated but gives a very good introduction to
    k8s.
  - Of course, nothing beats the documentation -
    [kubernetes.io/](https://kubernetes.io/).
  - If you later on plan on getting k8s certified,
    [Mumshad's courses on kodekloud are very nice for CKA/CKAD prep](https://kodekloud.com/courses/certified-kubernetes-administrator-cka/).
    You can also get the
    [notes for their courses on GH](https://github.com/kodekloudhub/certified-kubernetes-administrator-course).
  - Also the labs on [killer.sh](https://killer.sh/) are going to help a lot.
- You also need to learn a cloud provider. AWS is at top right now and I
  recommend studying it. If you're just planning to pass the certifications and
  have knowledge of AWS already, check out
  [Stephane's courses on udemy](https://www.udemy.com/user/stephane-maarek) or
  if you want gain in-depth knowledge, [Adrian Cantrill](https://cantrill.io/).
- For Jenkins, I used
  [Jenkins For Beginners In Hindi](https://www.youtube.com/playlist?list=PL6XT0grm_Tfi21F8O0TvHmb78P2uEmhDq)
  playlist and
  [Learn Jenkins! Complete Jenkins Course - Zero to Hero](https://www.youtube.com/watch?v=6YZvp2GwT0A).

Of course, at the end, no amount of watching videos will be enough and you need
to practice stuff on your own, say by Dockerizing your projects, doing bare
metal k8s installs, tweaking around the AWS consoles, working with GH actions
and GitLab CI/CD for learning CI/CD etc.

---

[`Source`](https://discord.com/channels/669880381649977354/1043921048841748591/1074714792348098680)

</blockquote>

`@sathyabhat` on developersIndia Discord (#devops channel) shared the following
advice on **upskilling in devops**:

<blockquote>

Look at [roadmap.sh/devops](https://roadmap.sh/devops) and start reading up.
From this, here's what I think you should do:

- learn a programming language. Any will do, python is good to start. You need
  to know enough to write small scripts, not just hello world
- learn to live in terminal: practice how to create files/directories,
  understand unix permission model (if I ask what does 644 or rwx-w--w- means
  you should be able to tell me)
- shell scripting is good to have
- learn about managing servers: how to install an OS, how to install software
  (pick any distro, I would recommend Ubuntu. Others the commands will differ,
  the principles will be the same)
- learn about how build, run software. Pick any open source software, or build
  your own, and learn how to package it to deploy. Write small shell scripts to
  make the 5 things you have to do always in to a script executable script
- learn about containers ("docker" is a tool, containers is the principle).
  Learn how to package this app you built into a container
- learn about CI/CD principles. Understand the principles. Tools like
  Jenkins/Gitlab/Github actions will come naturally. Practice how to build your
  app using CI principles. Then practice how to deploy them using CD.
- Understand how networking works. You don't have to go deep into the kernel
  level. At the minimum, you need to know about Subnets, routing, interfaces,
  ports
- Understand OS concepts: understand the Linux folder hierarchy. if someone asks
  you where the logs are, or how to get a app to run on startup, you should be
  able to explain these
- If you're going to pick up Cloud Skills: pick a Cloud, any cloud. Principle
  matters, implementation will come from reading the docs
- Understand fundamental pillars of cloud: IAM, Virtual networking
- build something in the cloud. Maybe a manually deploy that app you built onto
  a cloud VM
- learn some infra as code to automatically do these.

---

[`Source`](https://discord.com/channels/669880381649977354/670198758343966740/1075047326445469828)

</blockquote>

## Stories from the community

`u/Luci_95` on a post titled
[Switching from Software Developer to DEVOPS role](https://www.reddit.com/r/developersIndia/comments/1fjk7h5/switching_from_software_developer_to_devops_role/)
shared the following story:

<blockquote>

Switched from backend dev to SRE/Devops role now I'm back in dev.

Nothing concrete for the roadmap, but i polished my linux stuff. Unix and Linux
system administration handbook helped quite a bit. The firm was using aws at
that time with a few configuration management tools. Learnt ansible and puppet
to automates stuff. Monitoring tools like prometheus grafana basics of
alertmanager. Also brushed up my docker stuff later adding k8s to my knowledge
base. It was more than sufficient for the role that was needed.

Didn't have any prior experience as a devops engineer but I was already
containerizing my apps and deploying them on dev environments with proper
network and internal dns configurations so that was already helpful. Worked in
devops/sre for around 2.5 years post the transition

WLB would depend on the company and how many services you are running. I added a
decent amount of alerting to the services and the high priority ones always
needed some attention but then it would also depend on the app you're running
and how robust it is. Most escalations were due to minor miscommunications like
some environment variables missing and what not.

TL;DR I took up the role to be an actual fullstack dev in terms of coding from
scratch till deploying on prod. I think it's a skill every dev should have or
experience at least once.

---

[`Source`](https://www.reddit.com/r/developersIndia/comments/1fjk7h5/comment/lnot6k4/)

</blockquote>

`u/HHaunting-Plankton-55` on a post titled
[How to switch from Developer role to DevOps role? I am highly fascinated by DevOps roles, don't know why?](https://www.reddit.com/r/developersIndia/comments/1b585la/how_to_switch_from_developer_role_to_devops_role/)
shared the following personal journey:

<blockquote>

DevOps guy here. Switched form development to DevOps by learning myself. Great
salary, more than developers. They take a lot of interview but couldn't find
good guys. I did my last switch in Dec 2023 with 100% hike in very bad market.
Current salary 40 LPA. It's very exciting field, you will never get bored. There
is always something new to learn and try out. You get lot of power like admin
access to AWS and lot of systems.

Learn following tools :

git, A CI/CD pipeline tool, docker, kuberenetes implementation on any cloud,
ofcourse cloud and terraform + some monitoring and alerting tools,

This is lot to learn and rememeber, but if you could do it, there are always
jobs out there. AI cannot do what devops do, which is mostly setup, upgrade,
configuration, debugging, cost optimisation, automation, decommissioning of
resources.

To get interviews do end to end live projects and show it as your experince.
Most of the devops positions are 5+ years experience required.

---

[`Source`](https://www.reddit.com/r/developersIndia/comments/1b585la/comment/kt43odf/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)

</blockquote>

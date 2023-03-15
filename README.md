# Attacking & Defending the Software Supply Chain

---

## Goals of this training

The purpose of this training is to learn about the security posture of a specific software supply chain.   This training is not necessarily to compromise software supply chains, but instead to allow you to learn how a target writes, builds and deploys its applications.   From that insight will come an understanding of the weaknesses and attack vectors available against that target.  Given the right expertise, and time, this might allow you to compromise a targets software supply chain.

## Things you'll need for this workshop

1. Some familiarity with Git
2. Some experience with CI/CD processes 
3. Preferably a GitHub account, or you can make one on the day

## Who is the audience for this course?

There are several types of users that this talk could resonate with:

bug bounty researchers, pentesters and application security blue teams.

Bug bounty researchers will use black box techniques with little or no authorization to attack CI/CD resources.

Penetration testers will be similar to the above, except that they will generally have greybox or even whitebox access and therefore authorization and internal access to CI/CD 

Blue teams will typically have complete access to the internal, and external continuous improvement processes and workflows.  

## What is the software supply chain?

A software supply chain is the collective group of components that you need to have to create working software.  Said another way, the SSC is really anything that your application needs to successfully work.  

## What components make up the SSC?

Typically, this is defined as the components, libraries, assemblers, compilers, interpreters, frameworks, hardware, tools, software repositories, source code management platforms, build processes, testing and security tools that are used to develop, build, and publish a software artifact.  I will go one step further and say that the supply chain should also include the software engineers that build, maintain and deploy that software as well.  After all, the software supply chain encompasses anything that acts as a dependency or integral part of building working software, and if software engineers aren’t integral to that process, then I dunno what is!?

## Why do we need to attack & defend this supply chain?

Two facts are important to understand here.  First, the software supply chain is under growing threat.  These threats have [increased 600%](https://www.sonatype.com/state-of-the-software-supply-chain/open-source-supply-demand-security) or more every year since the start of the global COVID-19 pandemic.  There are orders of magnitude more threats spread across the software supply chain and the software development lifecycle (SDLC). These threats are often new and novel, with things like dependency confusion, repo name-squatting, and malicious package managers being new threat types.  The speed and scale that these threats have grown, are unlike any other IT related threat we have seen to date aside from ransomware.

The second fact is that software engineering and security teams are not keeping up with these new types of threats.  80% of software engineers admit to releasing software with known bugs, and 70% of engineers admitted to skipping existing security steps when under a time crunch.

Most importantly, our society now requires highly iterative software development lifecycles. Software bonds us all together, and our society has grown dependent on software that must evolve, and evolve quickly.   Understanding this, our society needs to make sure that software is scalable, secure and performant.  And the best way to do that is to use the same principles we use for all other important manufacturing processes that our society is dependent on:  We need to test it, and we need to test it thoroughly.  

And this means automation, and automation for software development is delivered via continuous integration and continuous deployment.


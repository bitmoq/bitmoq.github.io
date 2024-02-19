---
title: Embracing Salesforce DevOps
layout: blog
category: [Salesforce, DevOps]
excerpt: Do you need costly DevOps products to manage Salesforce DevOps? Well, let's explore how simple alternatives can help you achieve DevOps for Salesforce.
comments: true
---

Salesforce DevOps is the most discussed & wanted feature by all organizations that use Salesforce CRM. But have you ever wondered what is the right product and how to judge if that is the best fit? In this article, we will explore various DevOps offerings that are available, their advantages and disadvantages & what is best for you.

As of today, some of the most popular Salesforce DevOps products are:

1. **Copado**
2. **Salesforce DevOps Center**
3. **Gearset**

Apart from these products, there is also **an option to implement DevOps with traditional version control systems** like Azure, Github, Bitbucket and even Jenkins. If you are wondering why products other than those listed above are not featured in this blog, well it's not a coincidence rather it's a fact.

# 1. Copado

Copado has been a game changer in the salesforce DevOps space. Copado is built natively in Salesforce and hence offers all compliance, security and regulatory policies that Salesforce guarantees.

| Aspect                                    | Observation                                                                                                                          |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Price                                     | Very High (similar to Salesforce user licensing model)                                                                               |
| Best Suited For                           | Medium & Enterprise organizations                                                                                                    |
| User Friendliness                         | Excellent                                                                                                                            |
| Platform                                  | Built on Force.com Platform                                                                                                          |
| Learning Materials                        | Available on Copado Academy (similar to how Salesforce works)                                                                        |
| Credentials                               | Copado has its certifications (similar to how Salesforce operates)                                                                   |
| Features                                  | Pipelines, Environment Sync, User Stories, Quality Gates, Copado CLI                                                                 |
| Maintenance                               | As Copado is a managed package, it needs to be upgraded when new updates are available                                               |
| Need for a DevOps Team                    | Yes. Even though you get all these features, you need a qualified DevOps team to help teams manage releases & help resolve conflicts |
| Ability to extend the basic functionality | Yes. As this is a managed package, you can develop custom functionality on top of the objects Copado provides                        |
| Support                                   | Copado has an excellent customer support (similar to Salesforce)                                                                     |

As you can spot easily, Copado adopts the Salesforce business style and thus every aspect of Copado is very similar to Salesforce.

## What are the benefits of using Copado?

- As long as you have the money, onboarding and setup are very fast
- You can start with just 1 DevOps admin
- Since Copado is like the Salesforce king, customer support and guidance are very responsive. So, you won't feel lost.
- Their customer success team and account executives are highly responsive to your requests.
- They can provide you with certification vouchers and group discounts at will.
- Copado Academy has some courses that anyone can take free of cost but at the end, it will ask you to pay since the last module is a certification module.
- Their UI-first approach makes it easy for Developers and Administrators to use the product without any DevOps knowledge.
- Teams with clearly defined Agile/Scrum Project Management Methodology and have clear-cut visibility into what is delivered in a Sprint and what composes a Release + having a well-defined release cadence will love Copado.

## What are the pain points of using Copado?

- Even though Copado has lots of positives, it is not bulletproof. Some of the common problems are :
  - User Stories not syncing from any ALM tools to Salesforce.
  - Unrelated metadata appearing in commits.
  - Promotions getting stuck.
  - Environment Sync into Developer sandboxes sometimes rips out what developers have developed so far.
  - Any customized extension on top of Copado causing some hiccups is stamped as "Cannot be Supported" by the customer support team (so you will be hand-holded until they spot a customization & then you will be abandoned).
  - They recommend their partners to implement Copado for their customers (this can be a pricey affair).
  - Copado does not support JEST tests used for LWC (Lightning Web Components). So it is impossible to commit JEST tests. Copado recommends an ugly way to do so but it is not a standard/scalable approach.
  - Teams trying to mature their Project Management methodologies where ad-hoc priority changes derail what is scoped in a Sprint (that in turn affects your release cadence), Copado can be overwhelming. For example, Feature 1 is scoped to go out in Sprint 1 and Feature 2 in Sprint 2. Now, the business decides that the first part of Feature 1 and the last part of Feature 2 is of high priority and should be released in Sprint 1. It becomes challenging to strip out and attach individual pieces of functionality.

> **Words of Wisdom**: Copado might not be the best for Startups and Small Businesses when you are on the journey to stabilize your business towards profit making. Once you become a Medium/Large Enterprise, Copado will not feel expensive and hence it will look promising to your business.

Understanding the pros and cons of Copado will help you better prepare for what you are about to adopt. It's not a wrong thing for a product to have cons. Nobody is perfect but it is encouraging to see Copado is mitigating these issues in their product roadmap and maturing ahead. This is precisely why Copado is one hell of a competition in the Salesforce DevOps space.

# 2. Gearset

Gearset is a deployment solution for teams to compare, choose and deploy metadata across Salesforce orgs. A better way to say is '**Change Sets on steroids**'. Thus, it is not a pure DevOps product. So, why are we talking about Gearset when it is not a DevOps product?

Look at the value proposition. Gearset is best suited for teams who want to accelerate the deployment process.

Anyone who talks about DevOps is usually referring to automating deployments to salesforce org/environments. This part of automating deployments is just one aspect of DevOps and is called DevOps Developer Services. Gearset caters to the DevOps Developer Services layer of End-to-end DevOps offerings and that is why it is not a pure DevOps solution.

| Aspect                                    | Observation                                                                                                |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Price                                     | Low                                                                                                        |
| Best Suited For                           | Small & Medium Scale organizations                                                                         |
| User Friendliness                         | Good                                                                                                       |
| Platform                                  | Built out of Salesforce (it connects to Salesforce via OAuth)                                              |
| Learning Materials                        | Free of cost. Product Documentation & guide is available on their website                                  |
| Credentials                               | None                                                                                                       |
| Features                                  | Deployment, Sandbox Seeding, Backup, Automate Release, Support for CPQ, Revenue Cloud and Industries Cloud |
| Maintenance                               | Product and its features are maintained by Gearset. You have to maintain what you customize in Gearset.    |
| Need for a DevOps Team                    | No                                                                                                         |
| Ability to extend the basic functionality | No                                                                                                         |
| Support                                   | Mostly product documentation web page will have answers. On-call support is average.                       |

## What are the benefits of using Gearset?

- If your team has been using Changeset for so long and makes mistakes while promoting metadata, then Gearset can help make improvements in this process.
- Gearset has an easy and nice UI that shows you the differences in metadata between source org & destination org and helps make better decisions.
- Supports Git-based version control
- As it makes deployments easier, it does make rollbacks easier too.
- Gearset keeps a history of all the changes you make in the journey of promoting a change. Thus, it's easier to know what we did right and what did wrong.
- Automate deployments via pipelines.
- Support for data deployment.
- Support for Backup and Restore

## What are the pain points of using Gearset?

- Integration capabilities are limited
- Not for organizations looking to scale with a huge program plan & roadmap of projects running over each other
- The extent of customization supported is moderate
- Support experience is average

> **Words of Wisdom**: If you looking to accelerate Continuos Delivery across your Salesforce org, then Gearset is a good choice.

# 3. Salesforce DevOps Center

Salesforce DevOps Center (Salesforce's solution to DevOps) is a strong contender for all DevOps products and solutions out there. Even though this product is at its early stage and considering the speed of innovation at Salesforce, Salesforce DevOps Center will evolve soon to replace all other products like Gearset and Copado.

| Aspect                                    | Observation                                                                                        |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Price                                     | Zero                                                                                               |
| Best Suited For                           | Small, Medium and Large Scale organizations                                                        |
| User Friendliness                         | Excellent                                                                                          |
| Platform                                  | Natively available in Salesforce platform                                                          |
| Learning Materials                        | Trailhead (free of cost)                                                                           |
| Credentials                               | None as of now                                                                                     |
| Features                                  | Pipeline, Environment Sync, Git-based Version Control, User Stories, Release Management & Bundling |
| Maintenance                               | Product and its features are maintained by Salesforce. You have to maintain what you customize.    |
| Need for a DevOps Team                    | No                                                                                                 |
| Ability to extend the basic functionality | None                                                                                               |
| Support                                   | Standard Salesforce Support used for Salesforce customers                                          |

Setting up the Salesforce DevOps Center is very easy and requires very little technical know-how to do so.

## What are the benefits of using Salesforce DevOps Center?

- Supports user story-based development
- Supports scratch org or sandbox development model
- Easy to setup
- No code & configurable product
- Admin & Business User friendly
- Developer-friendly (VS Code IDE)
- Supports all Git-based Version Control Systems
- Ability to bundle user stories into a release
- Shows how much an environment is out of sync and helps resolve that
- No need for a DevOps Team. Your Salesforce Admin can manage this on their own.

## What are the pain points of using Salesforce DevOps Center?

- Rollback capability is missing (it will soon be addressed by Salesforce)
- Scheduling a deployment is missing
- Automatic deployments are missing
- No support for Quality Gates as of today

> **Words of Wisdom**: Do not underestimate the power of the Salesforce DevOps Center. It will evolve as the king of Salesforce DevOps and rule out every other product in the market very soon.

# 4. Traditional YAML Pipelines

If you are an organization that uses Azure/Github/Bitbucket for other tech stacks and still uses Salesforce for CRM needs, leveraging YAML pipelines in your existing Version Control system might be a good choice. The reason we said "might be" is because with Salesforce DevOps Center natively being offered free out of the box in the Salesforce CRM, you can leverage Salesforce DevOps Center for Salesforce CRM-related development & enhancements and use traditional YAML pipelines for other tech stacks. This technique reduces the need to set up a full-fledged DevOps setup in YAML for Salesforce.

| Aspect                                    | Observation                                                            |
| ----------------------------------------- | ---------------------------------------------------------------------- |
| Price                                     | Depends on whether you have in-house expertise or not                  |
| Best Suited For                           | Small, Medium and Large Scale organizations                            |
| User Friendliness                         | Developer friendly. Not for admins or business users                   |
| Platform                                  | Pipeline features are available natively on the Version Control System |
| Learning Materials                        | Have to depend on community blogs/posts, YouTube videos, etc           |
| Credentials                               | None                                                                   |
| Features                                  | Any feature can be developed, provided the right experts work on it    |
| Maintenance                               | Very Low                                                               |
| Need for a DevOps Team                    | Yes                                                                    |
| Ability to extend the basic functionality | Highly Extensible                                                      |
| Support                                   | Your own DevOps Team should support this                               |

YAML Pipeline is not a full DevOps setup. It will only bring CI/CD (which means validation & deployment across Salesforce org by still maintaining a history of changes in branches existing in Version Control Systems). You definitely can add more jobs and steps in your YAML pipeline to add code analysis, linting, automation tests, etc.

Getting this done in YAML for Salesforce is a bit different from how you do code validation & deployment for C#, Java, and NodeJS projects. Apps developed on programming languages like C#, Java, NodeJS, etc all have compilers locally on your machine. But for Salesforce, no apex code or out-of-the-box configuration can be compiled locally. It all has to be saved/compiled on the cloud platform directly. Therefore, the approach fully changes.

This is why having the right experts to do this setup is very important. We have heard stories of organizations where their app teams who successfully developed pipelines for React-based projects were asked to do Salesforce pipelines and they entirely screwed it up. Right experts mean Senior Architects/Leads/Organizations specialized in Salesforce Cloud with rich experience in DevOps.

## What are the benefits of using Traditional YAML Pipelines?

- Highly scalable & extensible
- Ability to add more steps in your DevOps process (like quality gates, linting, code analysis, etc)
- Leverages Git-based Version Control System
- Any functionality related to Salesforce CI/CD can be developed
- Environment Landscape (if done rightly) can be used to migrate from Traditional YAML pipelines to any other DevOps products

## What are the pain points of using Traditional YAML Pipelines?

- Requires the right experts to set this up for the first time
- Requires a Salesforce DevOps team to maintain and manage the health of pipelines
- YAML pipeline-based DevOps is only developer friendly but not admin/business friendly
- Support is very limited hence this is custom development and very less blogs/articles are there

# Verdict

- **For Startups and Small Scale Organizations**, the best choice is Salesforce DevOps Center for Salesforce CRM
- **For Medium Scale Organizations**, the best choice is Salesforce DevOps Center/Gearset for Salesforce CRM & Traditional YAML Pipelines for other tech stacks
- **For Large/Enterprise Scale Organizations**, the best choice is Copado for Salesforce CRM
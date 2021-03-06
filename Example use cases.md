# Example use cases

These example use cases tell stories about companies and the problems they were able to solve with Cloudomation. If that is not what you are looking for, you can find code for example automation scripts [here](/documentation/Examples).

As a general purpose automation tool, Cloudomation can be used for a wide range of use cases. We tried to find some examples from different industries and applications to provide an impression from different perspectives. We recommend you find a use case that you can relate to and start there, instead of reading from top to bottom. Each use case starts with a short description of its industry to make it easier for you to find one that is relevant to you.

If you have example use cases from your use of Cloudomation that you think might be a good example for others to learn about what Cloudomation can do, please reach out on info@cloudomation.io to share your story with us.

## The baker
<div class="parallax" id="bread")></div>  
This example use case describes a small bakery in a rural setting and how it could benefit from software automation to improve customer service and operational efficiency. In this use case, we left out most of the techincal details to make it easier to read.

Let us picture a small bakery with a handfull of employees. The master baker is proud of his breads and buns, of which he offer only a small selection, but all of them he makes himself. The bakery is situated in a small town that is just large enough to support a bakery, and the townspeople are happy that they can get fresh, local bread from their own bakery around the corner.

Most of the baker's business is with locals who are regular customers. Because many of them take the trip to the bakery for fresh rolls on the weekends for a special breakfast, few can do so during the week when they have to work. So the baker decided to offer a bun delivery service for the town.

It is a big success - most of his regulars, and many new customers come to the bakery to sign up for fresh delivery of bread a buns during the week. Soon, the baker realises that he underestimated the administrative effort that comes with this service. He is happy to bake the bread and buns and enjoys the increase in sales it brought, but soon he finds himself sitting until late in the evening to make lists of what to order for the early morning delivery of ingredients for the next day, lists of what he has to bake, and where to deliver it. And at the end of the first month, he has to hire help to go through all the notes from the entire month to draw up the right invoices for each customer.

What he had underestimated was that everybody wanted something different, and people change their mind. So one day, a customer comes in and asks for two white buns to be delivered every morning, Monday through Friday. But the next day, he calls and wants a danish in addition to the two buns for the next day. And after a week, he calls to say that he will be on holiday and won't be needing any deliveries for the next two weeks. Other people come into the store and change their order, others talk to him on his delivery rounds - and soon he has a mess of notes everywhere and no overview of who wants what when.

After the first month, he decides that he either has to quit the new delivery service again, or hire a new person to deal with the administration of it - which would cost him more than he makes with the delivery service. Or - he has to find some other way to manage his customer's orders.

Luckily, his nephew is studying informatics and suggests that the baker could automate the entire ordering process. The baker is sceptical at first, but willing to give it a try. After all, he doesn't want to stop his new delivery service just because he can't find his way around all his notes.

So his nephew sets up a very small web form on top of the Cloudomation INPUT function for the baker's customers. Customer can log in to see their orders, change them, and place new or additional orders. It is a very simple interface, but it is enough. And what's more: for those customers who don't want to use an online interface, because they don't have a computer, or don't like using it, the baker can use it himself to make things easier. He can go to the interface on his phone when customers talk to him on his delivery round, or he can use it on his tablet when they come to his store or call him. He just inputs what they want, and doesn't have to worry about it anymore.

The baker soon starts to use the interface for his own planning as well: he inputs what he wants to bake when, and now has one place where he can see everything he has to bake each day, the ingredients he needs to order, and

With Cloudomation, the baker's nephew automates the order processing: ingredients for the early morning delivery are placed with the click of one button, the baker just checks it before he sends it off. His nephew offered to automate it fully, but the baker prefers to have a last look before he places the order. Each morning, he can look at the list of things he has to bake, and how he should package them up for his delivery. As a small goodie, his nephew added a small feature that creates a map with the best delivery route for the baker. And at the end of the month, invoices are sent out automatically without the baker ever having to worry about it. It checks if the money is paid, and if it isn't, sends out reminders. The baker can see who has paid, who is still owing, and how much each of his customer's has spent with him.

As a next step, the baker wants to integrate the workflow with his cash register software. His nephew said it would be easy, and it would allow him to automate large parts of his cashflow management with Cloudomation.

In the end, the baker is glad that he can keep his delivery service, as are his customers, who are happy about fresh bread and buns each morning. The baker also is proud that he is using modern technology in his business. And in the end, he is much happier about having paid his nephew a few days of work to set it all up, instead of having hired someone to do it all manually.

The baker knows that he could not have set it up himself, but his nephew told him that Cloudomation also has a lot of partners that could have done for him what he did just as well. There might even be a Cloudomation partner specialised on bakeries one day.

His nephew goes on to tell the baker that he could now easily expand into the neighbouring town, open a new shop there, and double his revenue by delivering fresh buns and bread there as well. But that is one step too much for the baker, he is happy in his town and prefers to leave the neighbouring town to the neighbours. So his nephew posts his automation flow scripts into the Cloudomation public flow script library where other bakers could use it if they want to set up a similar delivery service.

## The software company
<div class="parallax" id="code")></div>  
This example use case is about a small software company and how it uses Cloudomation to set up continuous integration in their software development process. They improve their operational efficiency and reach operational excellence that allows them be more confident in their product, and focus on what they are best at: developing great software.

Let us picture a small software company with a dozen employees and a few years in the market. They have grown organically  and while they have come a long way since the early days where it was just the two founders, they still often feel like there is too much to do, too little time, and that they could easily keep twice as many people busy.

One day, the lead developer, who is also responsible for the software build whenever they release a new version, suggests to approach automation more professionally. He has automated bits and pieces here and there, with small bash scripts that he has to tweak manually for each build, as each one is slightly different, and has found that he spends much more time maintaining his growing jungle of small bash scripts than he had anticipated. Automating in this way is not saving him nearly as much time as he had hoped. But he believes in the power of automation and has long lobbied for taking it more seriously.

The CTO, as always, is all for the idea in principle, but doubts that there are proper solutions out there that fit their budget. He has heard of the "big boys" in automation, large software companies use them for continuous integration. But that has always been a distant dream, something they would have to spend years and millions of euros to set up.

Luckily, the lead developer had heard of Cloudomation. The CTO agrees to sign up for the six week free trial, but insists that product development has to take precendence. Automation should only come if and when there is time at the end of a sprint.

The lead developer agrees, and signs up for Cloudomation on the same day. That evening, he sits down and starts putting some things together. Using scripts from the public flow script library, he is able to get the first step set up within a few hours: a flow script that integrates their version control system with their build automation tool. He had tried to do this before, there are plugins available, but had not been able to set it up smoothly.

He is taken by Cloudomations functionality that goes far beyond the simple integration of git and Jenkins (for example). He is quickly able to figure out that, beyond the build, they could use it to deploy and configure fresh VMs from scratch and deploy the latest build there, removing the need to have environments ready and prepared before running a build. They could also use it to automatically deploy bug fixes to all their customer's instances. And he could use it to finally modularize and parameterize his install script into reusable pieces, which would reduce his effort for adapting the install script for a new version immensely.

But - step by step. He is happy that he was able to set up the version control and build automation integration so quickly. This would already be useful.

The next day, he shows his colleagues his new integration and they agree to test it. On the first day, they already find two bugs that led to the build failing. Before, they would most likely only have noticed whenever they would have decided to make a new build, which is some work, so they only did it at the end of each sprint. And when the build fails, the arduous task of root cause analysis starts - which commit was it that caused it? Go back far enough to find out, fix it, only to realise that three commits later, it fails again. Now, they knew right away where it failed, and are able to fix it right away, saving the lead developer hours of work - work that he disliked.

Soon, a colleague asks if they can add the testing to the pipeline. Right now, a commit only triggers the build. So when the build fails, they know right away. But what about the other tests? The lead developer agrees, they should do it as soon as possible. But he had promised the CTO to go slow, so he waits until the end of the sprint.

At the end of the sprint, the build runs without issue and he suddenly has half a day that he would usually reserve for bug hunting at the end of the sprint. So instead, he spends that half day to add the testing suite to the pipeline.

At first, it is painful. Most commits are rejected. But soon, the developers themselves realise how much quicker they learn. They get immediate feedback! They start pushing their code more frequently, and find bugs before anyone else touches their code. The shameful realisation that it was their commit that caused that ugly bug becomes a private learning. Enabled by the rapid feebdack and painless build and test cycle, developers become more confident, and releases become much more stable.

At the end of the second sprint, the system administrator discovers Cloudomation. She starts to play around with automatic environment configurations and automatic health checks for customer environments.

Soon, they reach the limits of the free Cloudomation trial. When they go to the CTO to ask for budget to upgrade to a paid plan, they have their arguments laid out: time saved in bug fixing, vast improvements in development, and the system administrator thinks that she can slash their cloud bill by twenty percent once they automate the provisioning of their dev, qa, hotfix, and feature environments. Just by shutting them down when they are not needed they would save boatloads. And with Cloudomation, it would be possible - because spinning them up again would be a matter of minutes, triggered by one simple command.

The CTO doesn't take long to convince - they had him when the lead developer admitted that it had already saved him half a day after the first sprint. Now, they spend the time they save to iteratively add to their automation pipelines. The lead developer enjoys developing reusable flow scripts much more than writing one-off installation scripts for each version of their software. The system administrator feels for the first time that she has a handle on her workload, and goes to bed with a calm mind - if something happens, she will be notified and not find out in the morning that all hell broke lose while she was asleep. And bit by bit, each person in the twelve people team starts to use Cloudomation for their own little tasks.

If you feel like the system administrator, build master, or one of the developers in this story, reach out to us at info@cloudomation.io. We are happy to help you convince your boss that Cloudomation will increase your productivity.

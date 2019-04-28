# Hooray GA!

GA is short for General Availability, which is nerd slang for the first publicly available version of a new software. It is an important milestone in the life of a software product - and it marks the start of an entirely new chapter.

Software is never quite finished but constantly changing and growing. GA marks a point of maturity where we judge Cloudomation to be so stable, secure, and feature-rich that it can provide real value to its users. However we are only just getting started and still have a long way to go - what you are still missing in Cloudomation (and the website) is probably already being planned or implemented by us!

To make sure that we focus our efforts on the things you really want, please let us know what it is that you would like us to focus on. Drop us a short email with all your wishes and feedback to [info@cloudomation.io](mailto:info@cloudomation.io).

What we ask of you is to be honest and gentle. Tell us where we still need to improve, and tell us in a way you would tell a small child: with a clear view on the potential within, and the aim to provide helpful guidance for the future. We appreciate your candour!

In turn, we solemnly promise to shape our fledgling product with enduring love and patience, guided by your wishes.

## What version 1 has in store for you

Despite its youth, Cloudomation is already quite a versatile and hefty solution. Let me draw your attention to a handful of its features. Review the [benefits](/Benefits) and [functionality](/Functionality) pages for a more high-level overview.

#### Git integration.
<img src="/sitedata/images/git-logo.svg" alt="git logo" class="responsive d-none d-md-block" style="float:right; margin: 10px 20px"/>
Git is the most popular and most widely used version control technology of today. In software development, using version control is almost as fundamental as using a computer. Cloudomation wants to support you in attaining operational excellence, which is much easier to do with efficient automation. As a consequence, we also want to enable you to use good processes when developing your automations. This starts with using version control also for the development of your automation scripts, which we call flow scripts.  
Cloudomation features a GIT task type which allows integration with any git system (public or private, github or any other git-based version control system). There are also example flow scripts available in the [public flow script library](https://github.com/starflows/library){ext} that exemplify the [synchronisation of flow scripts and settings](https://github.com/starflows/library/blob/master/configure_webhooks_github_cloudomation.py){ext} from a github repository to Cloudomation.  
Integration with git doesn't *just* enable you to use version control for flow script development. It also enables you to plug automations into your software development process - such as automatic tests or build processes triggered by git commits, or automatic notification systems for pull requests, merges, and other activities on your git repositories.  
In short: git integration is your starting point for building a full continuous integration pipeline with Cloudomation.

#### Transaction safe automations.
<img src="/sitedata/images/transaction_safe.png" alt="transaction safety icon" class="responsive d-none d-md-block" style="float:right; margin: 10px 20px"/>
Such a mouthful - and such a wonderful thing! Transaction safety means that your automations can be paused during execution, and restarted exactly at the point of interruption at a later time. Might not seem like much, but it is in fact a *lot*.
It means that you can gracefully handle all the unexpected things that always happen when you deal with software. Say there is a server that just doesn’t respond. Your automation relies on that server. What do you do? You wait. Your automation doesn’t crash, it just - stops. And then you have all the freedom to decide what to do. You can trigger diagnostics and repair processes (hint: via Cloudomation). You can send out notifications. Or you can just wait and try again after a few seconds. Maybe the server has recovered by then and your automation will finish.
Still doesn’t seem like much? Ever decried the loss of data because of a software crash? Ever wondered at what exactly has already happened, and what hasn’t happened, when a script of yours just fails - somewhere? (Of course you haven’t. You always log everything conscientiously. Don’t you? Guess what: Cloudomation does that for you as well.)
Transaction safety enables you to elegantly handle errors. Be a hero and design self-healing processes. Cloudomation gives you all you need to do just that. It’s not just a fancy word. You can actually do it. Quite easily. With Cloudomation.
And as a side effect, you have a full audit trail: at each point in time you know exactly where your automations are. If they do stop you know exactly where they stop and what the last command was they executed. And when you resume them, they don’t redo anything they have already done. They just start again exactly at the point where they were stopped.
You know what else this means? You can take your executions at runtime and just put them somewhere else. You can pause executions to free resources if you are running too many things at once.
In short: you get a whole new set of options for amazingly efficient and robust handling of your automations.

#### Last but not least: Python!
<img src="/sitedata/images/python-logo-generic.svg" alt="Python logo" title="&quot;Python&quot; and the Python logos are trademarks or registered trademarks of the Python Software Foundation." class="responsive d-none d-md-block" style="float:right; margin: 10px 20px"/>

We are big fans of Python, a language that has made programming accessible to swathes of people through its readability, low learning curve, and enthusiastic community. Automation scripts for the Cloudomation platform, which we call flow scripts, are written in Python. This brings three huge benefits: (1) there are many people who already know it and who don't have to learn anything new to use Cloudomation, (2) there are a LOT of community resources out there to help you learn and improve your Python without relying on us, and (3) you can extend your flow scripts with standard Python functionality.  
My personal favorite is number (3). It exemplifies some of our principles. It empowers you, the user. It enables us to focus on what we're good at: providing automation-specific functionality - we don't have to implement if clauses, enumeration concepts, regex matching, or any other functionality that already exists in Python, because it's already there for you to use. We provide the very specific value add for automation. Nothing more, and nothing less. And finally, building on Python functionality allows for a jump start followed by iterative improvements. Because so much is already there, you can build powerful and complex automations already with the very first version of Cloudomation. And as Cloudomation matures, we will add more automation features (which are transaction safe, scalable, and comfortable to use) which will make your automations simpler, safer, and more stable, step by step.

#### Tell us what you think!
I could go on to tell you about all our other amazing features - secure connections to remote systems via ssh, interaction with web interfaces via REST, interaction with humans through input requests and emails - and so on and so forth. But I don't want to strain your patience. Instead, I want to invite you to try it out yourself. Create your six week free trial account now at [cloudomation.io/signup](https://cloudomation.io/signup) and see for yourself. Feedback is welcome and appreciated: tell us at [info@cloudomation.io](mailto:info@cloudomation.io) what you liked, what you disliked, and where you think we can do better.

Now all that remains to say is: Rejoice, the bliss of automation is at your fingertips!

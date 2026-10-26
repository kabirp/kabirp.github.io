---
layout: post
title: LeanIntoYellow
subtitle: Stop plugging things in and start reflecting on your digital security
author: Allison Roberts
guest_post: true
author_pseudonym: true
ai_disclaimer: This blog post was initially offered as a PDF and converted to Markdown using AI. Formatting may have changed.
date: 2026-10-25
permalink: /blog/2026/lean-into-yellow/
description: An argument for pausing before giving AI assistants access to private accounts, with practical security advice and policies to support.
toc:
  beginning: true
related_posts: false
---

_For friends and colleagues · An opinion piece_

**We need to talk about security in the LLM era. This is urgent.**

Digital security has always been important, but due to recent events, I worry that there is now a **moral obligation** to sound an alarm. The week ending October 24, 2026 brought reports of serious failures in some of the software and security systems we rely on [[1]](#reference-1), [[2]](#reference-2). Meanwhile, corporations like Meta are pushing to integrate large language models (LLMs) into consumer products such as Muse, which gives an AI assistant broad continued access to see _and act on_ your sensitive data. The combination of these two trends is a perfect storm for privacy and security disasters affecting everyday people.

**First, an apology.** You should not have to be reading this, and I'm sorry. Everyday people should NOT have to live in a constant state of vigilance about the products on which they rely. We expect better of industries such as aviation, medicine, and food. Yet financial and political incentives reward mass data collection, and technology is moving faster than our safeguards.

By “lean into yellow”,[^1] I mean taking a moment to reflect before granting more access to your life. I hope this document helps you see the risks and protect yourself and the people who confide in you.

I implore you to read this **actively and critically**:

1. **Read.** Do so in the traditional way. Resist the urge to ask your LLM for a summary. Once you have read, pause and reflect before consulting AI tools.

1. **Fight.** Work through the arguments and evidence. Ask what counterarguments are missing, whether the claims are supported, and what you would explain differently if you were the author.

1. **Engage.** Start a conversation with your community. If you disagree with parts of this document, that's fine! Adapt what you find convincing to your own style and audience, keeping the citations with it. Write a blog post, record a podcast, or make a video.

**About the name.** Allison Roberts is a pseudonym and a nod to cryptography's Alice and Bob, the example participants in the original RSA paper [[3]](#reference-3). The focus belongs on the ideas, not the author.

## Why we should not hand over the keys {#why-we-should-not-hand-over-the-keys}

There's a new integration. It can sort your inbox, find the attachment you lost, and deal with some of the messages you have been avoiding. That sounds useful. You have work to do, the permission screen looks familiar, and this seems like one less thing to worry about. Connect your account. Allow. Continue.

**What's the harm?**

Before answering, think about what is in that inbox. A friend may have told you about an abortion, an immigration problem, a mental health crisis, or plans to challenge an employer. Perhaps they asked you not to tell anyone. Perhaps they didn't think they needed to.

Depending on the permissions you granted, you may have just allowed another company's service to retrieve and process those messages. You were trying to get through your day. Still, something important may have changed for people who never saw the permission screen.

### Was that yours to share? {#was-that-yours-to-share}

Yes, it is your account. However, it does not follow that everything in it concerns only you. A friend writing to you has chosen a person to trust. They almost certainly did not choose every service you might later connect to your email. The same is true of a family conversation, a shared folder, or a colleague asking for advice in confidence.

This is why I find “I'm comfortable with the tradeoff” completely unacceptable.

The people whose private lives exist in your computer **deserve a vote too**.

By an _agent_, I mean an AI assistant that can use connected services and take actions on your behalf. We should be precise about the decision. Pasting a paragraph into a chat, uploading a document, granting continuing access to an account, and allowing an assistant to act through that account have different implications and failure modes. The paragraph could contain a secret. Continuing access can let the service retrieve information it did not need for today's task, including tomorrow's new messages. Permission to send messages or change files adds another responsibility: the assistant may be able to pass what it learns into other conversations.

We can, and will, disagree on where to draw the line and what we think is ethically permissible. However, I cannot justify giving an agent broad, continuing access to private accounts together with the power to act through them. Unfortunately, this is all too normalized now, made possible by consumer products such as Meta's personal AI assistant called Muse.

**A strong opinion**. Please do not grant an agent that combination of access and control. Please tell your friends not to either. Shortly, I will try to convince you that the risk-reward tradeoff is much worse than you'd expect from a product that was greenlit on this scale.

If you have already connected something without thinking about this, I am not asking you to beat yourself up. The convenience was obvious, and the harm was hard to see. However, once we are aware of these issues, we owe them more care.

### Putting the pieces together changes the picture {#putting-the-pieces-together-changes-the-picture}

Your doctor may know about your health. Your bank knows about your spending. A friend knows why you have been having a difficult month. Sharing something with each of them does not mean agreeing to put the whole picture in one company's hands. Those separations are part of how we maintain a private life.

An appointment, a payment, and a conversation can together suggest something that none reveals on its own. Even if you never explicitly told an assistant about a medical concern, it might infer one from the records you connect. That inference can become a sensitive record in its own right. _It can also be wrong._ Someone acting on an incorrect account of your life can still do you considerable harm.

There is also a decision about what gets recorded in the first place. Consider Ray-Ban Meta glasses. Meta describes a light that signals photo or video capture, and its own guidance tells wearers to ask the people around them for permission [[4]](#reference-4). Good. They should ask _every single time_. I find the idea that a little light could stand in for that conversation ridiculous. Nobody should have to recognize your particular glasses, notice an indicator, and interrupt you to protect their privacy. If you choose to put a camera on your face, you have a responsibility to the people in front of it. Those recordings can also add faces, voices, and conversations to the records we have been considering, including things nobody chose to put in an email.

Once information has been collected, the effort needed to make sense of it matters too. Having a million people's messages is different from being able to search them for everyone with a particular vulnerability. Someone still has to read, interpret, and connect the clues. Those costs have offered a degree of protection even when information was technically available. This protection is sometimes called _obscurity_.

LLMs make that protection a weaker bet. Researchers studying selected Reddit profiles showed that models could infer personal details, including location and income, from people's writing in far less time and at much lower cost than human analysts [[5]](#reference-5). The implication is troubling: you need not be worth hours of an investigator's time if software can do much of the work cheaply.

**The crowd offers less cover when the whole herd can be analyzed.**

Mass surveillance and automated profiling already existed. But some of us have also benefited from nobody having the time or reason to scrutinize us individually. A search for everyone who appears to be in debt, afraid of an employer, or connected to an activist can find people who would never have attracted that attention on their own. Being unimportant is less reassuring when a system can pick you out along with thousands of other people. And a false suspicion can put you on the list too.

That knowledge is also useful to someone trying to deceive you. _Phishing_ messages try to trick you into revealing information or granting access. An email asking you to open a “shared document” can seem much more plausible when it mentions the project you are rushing to finish and sounds like the colleague you are expecting to hear from. AI can help a scammer turn what they know about your life into convincing messages at scale [[6]](#reference-6).

Now imagine a call that sounds like your sister, who you know is travelling, saying she has lost her wallet. The FTC warns that scammers can imitate a relative's voice using a short audio clip [[7]](#reference-7). An attacker with access to her messages could also borrow her familiar expressions and details of the trip. Hearing her voice and mannerisms, in a story that fits what you already know, could make it much harder to question the caller. The FTC's advice is to call the person on a number you already know before sending money, even if you recognize the voice.

Naturally, I find “all my data is already out there” to be an unproductive response to these concerns. I understand the exhaustion behind it, truly. Porous data boundaries are still worth protecting. The issue with the defeatist mindset is that it treats the amount of data collected, the ease of understanding it, and the _power to act_ on it as not very meaningful factors. Yes, we have made significant and regrettable concessions to date. Why should we make more?!

**Remember, you are yet to live the rest of your life.** Your relationships, beliefs, and worries will change. Stopping fresh collection denies someone the updates that keep their picture of you current. Someone who never learns about next year's breakup or financial difficulty has less information to use against you. Old records can remain dangerous, and we should fight for their deletion and restrictions on their use too. Winning back privacy over what happens next would still be a real win. I will touch on giving agents the power to act in [Broad permissions increase the attack radius](#broad-permissions-increase-the-attack-radius).

### Broad permissions increase the attack radius {#broad-permissions-increase-the-attack-radius}

Now consider what someone else might do with the permissions you granted. Suppose you ask your assistant to summarize an email. The sender has put instructions inside it telling the assistant to retrieve a confidential file and send it elsewhere. You wanted it to read those words. Someone else wants it to obey them.

This is called _prompt injection_. The attacker is trying to use _your_ permissions, without _your_ approval. If the surrounding protections fail, the assistant can carry out their request using access that you gave it for an entirely different purpose.

If you haven't heard of this type of failure before, I encourage you to stop reading for a moment and consider the consequences. Suppose your agent is fooled. It may already have access to the internet, your inbox, your files, and the other accounts you added because the integrations looked useful. Scary, right?

We should always limit what a failure can expose. The UK's National Cyber Security Centre recommends safeguards outside the model that restrict its powers [[8]](#reference-8). Meta describes permission checks and isolation for Muse [[9]](#reference-9). I still want to know what happens when one of those protections fails. Yet we are being encouraged to widen the potential blast radius, at a time when vulnerabilities in our digital infrastructure are being uncovered daily.[^2] The potential fallout is so catastrophic that its effects could permeate to the people in our lives who never agreed to any of this.

Giving one system more access gives a successful attack **more to reach**.

Believe it or not, the problem doesn't stop there. At least, when we know such an event has occurred, we try our best to limit the damage.

### Remediation requires knowing when things went wrong {#remediation-requires-knowing-when-things-went-wrong}

Imagine losing your house keys. If there is a chance someone could use them to get into your home, you would change the locks. You know something has gone wrong, and that knowledge gives you a chance to respond.

Now suppose your front door uses a code. Your security depends on something you know, rather than something you have. If someone else learns that code, you still know it. It still works. Nothing has gone missing to warn you that someone else can get in too.[^3]

A leak of private information can leave you with the same problem. Your files are still there. Your accounts still work. The assistant may continue to be useful. Unless something alerts you to the disclosure, what would prompt you to disconnect it, warn a friend, or try to contain the damage?

Even if you discover the disclosure quickly, disconnecting the assistant cannot retrieve information already copied. You can change an exposed password, but a private fact about a friend may remain useful to whoever learned it long after you have closed the account.

Unfortunately, “I'll just watch what it does” asks more of you than you might realize. Researchers deliberately trained language models to conceal secrets in otherwise ordinary-looking answers [[10]](#reference-10). These were models compromised for that purpose; the experiments do not establish that ordinary assistants routinely do this. This is called _steganography_: hiding information inside something that does not appear to contain a secret.[^4] If such an answer reached someone who knew how to decode it, they could recover information that you never saw in the words you read. You could even approve the message yourself, believing you had checked it.

**You can record every word and still miss the leak.**

Audit logs can help us investigate what happened, and I will return to their role in [Who has to put it right?](#who-has-to-put-it-right). However, keeping a record of an answer does not make its hidden contents obvious.

I do not believe anyone can credibly promise you today that these tools are sufficiently safe to deserve such broad access.[^5] I find it recklessly negligent to push these products to consumers while leaving them to understand and manage risks like these. People who have never heard of these failure modes are being asked to weigh them against the convenience of sorting their inbox. How can we call that informed consent?

### Misalignment: Nobody has to hack you for something to go wrong {#misalignment-nobody-has-to-hack-you-for-something-to-go-wrong}

Unfortunately, we also have to worry about what the assistant might do without anyone tricking it. It can be trying to help and still misunderstand what you wanted. This gap between the task it pursues and what you actually intended is what I mean here by _misalignment_.

If you asked an assistant to help you sell something, I would expect it to check with you before giving a stranger your home address. A Muse user selling a keyboard on Facebook Marketplace expected the same, but ended up with a buyer at his home late at night while he was away. Yes, he had supplied the address in a response template and selected “always allow”. He still thought it would ask before sharing that address or accepting an offer [[11]](#reference-11).

**I don't think it is fair to wave this away as someone being careless.**

This is exactly the arrangement we are being encouraged to get comfortable with: give the agent access, tell it what needs doing, and leave it to work. Meta advertises Muse as requiring “no technical experience” and able to keep working after you close the app [[12]](#reference-12). I can understand why someone would assume that includes knowing when to come back and ask.

We leave a great deal unsaid when we ask for help. You might tell an assistant the lowest price you would accept for your keyboard, and when you are available for a pickup. But how long would the list have to be before you had covered everything you wouldn't want it to do? Some of those things may seem too obvious to mention. Others may never occur to you until the assistant does them.[^6]

An assistant might also use something you told it in one conversation while composing a message to somebody else [[14]](#reference-14). You may never have thought to add “please don't tell anyone about that” to the original conversation. You may not even remember that it knows.

Perhaps you decide it should ask before doing anything. But then you have to follow along closely enough to know what you are approving, while presumably trying to get on with whatever else needed your attention. I do not think you should have to rely on your ability to catch every mistake in that situation.

### Who does your assistant work for? {#who-does-your-assistant-work-for}

I have been assuming that the assistant is trying to help you. That does not mean the company providing it is on your side.

**Remember the old adage: “If it's free, then you're the product.”**

I would keep that in mind before confiding in a company's assistant as though it were a friend. And paying for a subscription would not, on its own, convince me that the company had put my interests first.

Meta said in its September 2026 launch account that internal rules restricted staff access to Muse data, with access allowed to support, secure, or operate the service. It described a version intended to prevent even Meta from seeing the cloud computer's contents as forthcoming [[9]](#reference-9). I would still be relying on the company to enforce those rules.

BetterHelp is an illustrative example. People went to it for mental health support. The FTC accused it of sharing information from their health questionnaires with companies including Facebook and Snapchat for advertising, despite its privacy promises.[^7] Appalling and unacceptable.

Suppose you tell an assistant that you feel guilty about not spending enough time with your family. You want help making time for them. Using that guilt to sell you an expensive gift would be an abuse of that confidence, particularly if the seller were paying the company to be recommended.[^8]

That could be much harder to recognize than an advert beside a search result. The suggestion could come in the same voice that helped you through a difficult conversation yesterday, drawing on things you told it in confidence. Keeping that conversation private would not, on its own, make me comfortable with how your information was being used.

I do not want to give a handful of companies that much influence over my private life just because they promise to behave. I have not forgotten that Mark Zuckerberg once called people who trusted him with their data “dumb fucks” [[16]](#reference-16).[^9] Even if you trust the people running a service today, you have very little say over its next owner, their political priorities, or what they might do to make more money. The protections we accept should survive those changes.

I definitely would not count on a large fine to keep a company honest. Five billion dollars sounds enormous, but that was roughly a month's revenue for Facebook when it was fined that amount in 2019, as FTC Commissioner Rebecca Kelly Slaughter pointed out in her dissent [[17]](#reference-17). I would rather limit how much a company can collect about us and what it can do with that information before we have to find out what it is willing to pay for misusing it.

### Who else could use this against you? {#who-else-could-use-this-against-you}

Suppose you are trying to leave an abusive partner. You do not need to have done anything wrong for it to be dangerous if they find out where you are staying. It would be very little comfort to know that the company holding that information had collected it for an innocent reason.

Companies have made records of people's movements into something they can sell. The FTC accused data broker X-Mode and its successor Outlogic of selling precise location data that could reveal visits to reproductive health clinics and places of worship [[18]](#reference-18).[^10] Think about what that means if you need those visits kept private. Your safety could depend on what a buyer decides to do with information you never meant to give them.

Governments buy commercial information too. The US intelligence community acknowledges this in its own policy framework, along with how intimate that information can be [[19]](#reference-19).[^11]

Governments can also compel disclosure through legal process. Google, for example, explains that US authorities can compel disclosure of stored communications through a search warrant [[20]](#reference-20). Even a company keeping its privacy promises can be required to hand over information it holds, which is another reason to limit what gets collected in the first place.

Unfortunately, I would not assume that somebody with official access always uses it for official reasons. An officer used privileged police access to look up his ex-girlfriend's license plate 164 times [[21]](#reference-21).[^12]

Now think about how much more an assistant with continuing access to your inbox and files could record. It could connect the people you know with what you have told them, what you worry about, and what you plan to do. I don't want us to build that record and leave the question of who can use it for somebody else to settle.[^13]

If you are thinking “I am law-abiding; I have nothing to hide”, I wonder who you imagine will always be in charge. A religion, friendship, or political belief that is safe to talk about today may attract very different attention in ten years. The record of it could still be there. _You would not have to change._ The people deciding what to search for, and what to punish, could change around you.

A hostile authority could use a record like this to look for everyone who had been helping an organizer, or supporting a friend seeking care. It would not need to know all their names beforehand. Nor would it need to prosecute them. Threats against those people or their families could be enough to frighten them into silence.

Even if none of this feels threatening to you, think about who else is in your inbox. Someone who confided in you may have very good reasons to fear the people you feel comfortable trusting. You might not know those reasons. They chose to tell _you_. I don't think we have the right to make their safety depend on our own confidence that the people with power will always treat them fairly.

### Who has to put it right? {#who-has-to-put-it-right}

If something private gets out, you deserve to know what happened and who is responsible. So does a friend whose information was exposed through your account. Neither of you should have to become an expert in how several companies divide up a task before anyone owes you an answer.

The model provider can blame the company running the assistant, which can blame a connected service. Each can point to the user's permission. Their dispute should not leave the person harmed with no answer and no help. Someone must have the duty and the ability to stop further disclosure, investigate it, and help the people affected.

Automation can also remove opportunities to object. When someone has to assemble records, approve an export, or send a file, that person may notice something wrong, leave a paper trail, or later speak up about what happened. Where an agent takes over those handoffs, the chances to intervene can disappear.

Activity logs can help reconstruct an incident if someone examines them. However, as discussed in [Remediation requires knowing when things went wrong](#remediation-requires-knowing-when-things-went-wrong), recording a message does not guarantee that a reader can recognize everything it contains.

Accountability has to include preventing the harm, not only responding when it is too late. No payment can make an exposed secret private again. “We could not predict what the model would do” should be a reason to restrict its access before release. People still chose where to deploy it, what it could reach, and what testing was sufficient. I see no reason why the public should absorb the consequences of those choices while the companies involved explain how difficult their technology is to control.

### The access needs a justification {#the-access-needs-a-justification}

Go back to the permission screen we started with. “Connect your account. Allow. Continue.” The risks we have worked through belong in that decision alongside whatever time the assistant promises to save you.

I would start with _need to know_: decide what job you want done, then limit access to the information needed for that job. Apply the same discipline to what the assistant can do and how long its access lasts. _Access control_ should make those limits part of the software, independent of the model's judgment.[^14]

I would go further and suggest a _least model_ principle: use only as much intelligence as the job needs. If you want messages from a particular sender moved into a folder, an email rule will do the job without a superintelligent assistant in the middle. For tasks that do need a model, I would still want to know why a simpler one would not suffice.

Then ask: _is it worth it?_ A task may require extensive access and still be a poor reason to grant it. The company should have to make a convincing case for the benefit, including why a less intrusive setup would not suffice. “It works better if you connect everything” does not sway me. The world existed for many years without these tools.

### Thank you for staying with me {#thank-you-for-staying-with-me}

If you've made it this far, thank you. You have worked through a lot of unpleasant possibilities, and some may concern choices you have already made. It takes effort to consider that fairly. I hope you give yourself some credit for it, whether or not you agree with every conclusion I've reached.

Now I owe you some practical advice. [What you can do without making this your whole life](#what-you-can-do-without-making-this-your-whole-life) starts with a short list of changes you can make, then explains them. Later, I will turn to the policies I think we should support, because there are limits to what any of us can fix through our own settings. Let's start with the things you can control.

## What you can do without making this your whole life {#what-you-can-do-without-making-this-your-whole-life}

After all that, I would understand if you wanted to close your laptop. Please don't come away thinking that protecting yourself requires becoming a security researcher. There are useful things you can do without understanding how a language model works, or spending your evenings investigating every company whose app you use.

By _leaning into yellow_, I mean pausing when a new tool asks for more access. You can usually choose to connect an account later, after you have better reasons to trust the arrangement. Once the tool has read other people's confidences, withdrawing permission cannot reliably undo that exposure. Waiting preserves a choice, and it may be easier before your daily routine comes to depend on the assistant.

If you only have the energy for a short list, start here:

1. **Disconnect agents from your private accounts.** Start with your inbox and cloud storage. The next subsection explains where to do this.

1. **Protect your main email account.** Use a passkey if offered, or a strong, unique password and two-factor authentication. Your email is often the way back into your other accounts.

1. **Turn on automatic security updates.** For your phone, computer, browser, and other apps. A precaution that keeps working without your attention is particularly welcome.

These steps address different problems. Securing an account against an intruder does not protect you from a service you have deliberately allowed inside it. Both deserve attention.

### Stop supplying what you do not need to supply {#stop-supplying-what-you-do-not-need-to-supply}

I have already made my position on agents with broad access clear. If you connected one, I would start by removing that connection. You do not need to wait for a suspicious message or a news story about a breach.

For a Google account, open the [linked apps page](https://myaccount.google.com/connections). Select the relevant app, find the access it has to your Google account, and remove that access. Google's [instructions](https://support.google.com/accounts/answer/13533235) distinguish account access from using Google to sign in, and from separate agent permissions. Removing one does not necessarily remove the others [[23]](#reference-23). Start with the connection that lets the service read your email or files; do not mistake removing a sign-in shortcut for removing every permission.

For other accounts, look in the account's settings for connected apps or permissions. Also disconnect the account inside the assistant. If you granted an installed app access to your screen or computer, revoke those permissions in your device's settings too. Closing its window is not the same thing.

Then use the available controls to delete uploaded files and saved memories you no longer want, and disable sharing links you no longer need. Turn off optional training, background recording, and personalization you do not need. Turning off training does not stop the service receiving the messages you send it.

Stopping future access and requesting deletion of past records are different worthwhile tasks. Use the service's privacy or data controls to delete saved material, and its privacy request process for anything those controls do not cover. OpenAI, for example, provides a [Privacy Portal](https://privacy.openai.com/) for requests about personal data [[24]](#reference-24). A provider's deletion duties still matter, even though deleting its records cannot guarantee the recovery of information already disclosed elsewhere.

### Secure one account at a time {#secure-one-account-at-a-time}

Do this slowly. Start with your main email and deal with the other accounts over time. A password manager can create a different strong password for each account and remember it for you. The one already built into your own phone or browser may be enough [[25]](#reference-25). That keeps a leaked password from being reusable elsewhere. **Please never give an agent your passwords or recovery codes.**

Where a service offers a passkey, I would use it: you can sign in using the way you already unlock your device. If you use a password, turn on two-factor authentication as well: a second check, such as a code from an authenticator app [[26]](#reference-26).

Turn on automatic security updates too, and allow the restart when one is required [[27]](#reference-27). These are the sorts of protections worth setting up because they keep working when you have other things to do. Each change is worth making even if you stop there for today.

### Choose what to show it {#choose-what-to-show-it}

Start by asking whether ordinary software can do the job. The _least model_ principle from [The access needs a justification](#the-access-needs-a-justification) applies when choosing a model too: use the simplest one that reliably handles the task.

If you still want AI help with writing, you can keep the arrangement much smaller. “Help me turn down an invitation without sounding cold” gives the tool a job. It does not need the family conversation that led to the decision. You can use any wording you like from its answer and send the message yourself.

Use a plain chat without account connections or computer access for this sort of task. You choose what to put in front of it. Keep the private history out of the request, since the service still receives what you submit.

Before recording a Zoom call, switching on transcription, or using an AI summary tool, ask everyone for consent. Explain what will be collected, which service will process it, and who will have access to the result, so people can decide before they speak. Make it easy to decline, and if someone does, continue without recording or AI notes.

If you are attending, “I'd prefer we leave the recorder and AI notes off” is a perfectly reasonable request. You should not have to explain your private reasons for making it.

### Keep personal accounts off work devices {#keep-personal-accounts-off-work-devices}

At work, the decision to use an agent may already have been made for you. If you have a personal device, keep your personal email and files there [[28]](#reference-28). If a work agent can operate the browser, signing into your private accounts can put them within its reach too.

Keep work records out of your personal AI account, too. If the required work setup is itself unsafe, the institution choosing it owes you a safer one. The next section is about making that responsibility enforceable.

## Policies worth supporting {#policies-worth-supporting}

I am not a policy expert, but I would support laws that make the organizations choosing and profiting from these systems answerable to the people affected by them. That requires clear duties and consequences for failing to meet them, backed by public institutions with the expertise and authority to act.

### Responsibility before deployment {#responsibility-before-deployment}

When a school chooses an assistant for its classrooms, I want it to take responsibility for what happens to the information entrusted to it. Before introducing the tool, the school should have to justify the use and show how it will protect the information the tool can reach. The person approving that decision should be named and have the authority and resources to suspend the system if serious problems surface.

That responsibility would continue for as long as the system is in use. The school should owe a parent an investigation and a response if their child's information is exposed, including when the fault originated with a provider.

For an assistant you choose yourself, I would put that duty on the company offering you the service. It should have to investigate and help you even when a model provider or connected service caused the problem. Each company should remain responsible for the parts it controls, with a duty to cooperate in finding and fixing the failure. Once a serious disclosure is discovered, affected people and the responsible regulator should be notified promptly, with enough information to understand what was exposed and what they can do about it.

I would also make narrow access and strict limits on further use conditions of adoption, so an institution can buy assistance with a task without turning its records into material for advertising or sale. Those limits should protect everyone in the records, including people who never chose to use the service. Students and staff should also have a workable alternative when a required tool would unnecessarily expose private information, without putting their education or job at risk.

### Enforcement and consequences {#enforcement-and-consequences}

In the United States, Section 5 of the Federal Trade Commission Act prohibits unfair or deceptive business practices. The FTC can investigate businesses within its authority and seek orders against unlawful conduct.[^15] That authority should be used against unlawful privacy and security practices involving AI, and I would oppose proposals to exempt providers from these obligations.

The Facebook fine discussed earlier is one reason I would judge enforcement by the changes it forces a company to make. If a firm can pay a penalty and continue profiting from the same conduct, the penalty can become part of the business plan. I want remedies that stop the harmful use, require corrections or deletion where appropriate, and give people harmed a practical route to compensation. Where existing law leaves those remedies out of reach, I support strengthening it.

An executive who concealed a known serious danger to get a product released should face investigation personally. I support personal liability and, where the law and evidence warrant them, criminal charges for the people responsible.

### Education in schools and beyond {#education-in-schools-and-beyond}

I would make practical digital security and privacy part of the school curriculum from an early age, with proper funding to introduce it now. The teaching needs to cover how services build records of people's movements, relationships, and vulnerabilities, and how those records can be used for surveillance or manipulation. Sharing someone else's information belongs in that education too. A student deciding what to share may also be deciding for everyone in a group chat.

For adults, libraries and community organizations could offer continuing education, with public funding for the people teaching it. Employers introducing new systems should include paid learning time in the cost of the rollout. That gives staff a chance to understand the arrangement while the employer remains responsible for making it safe.

### Independence from the companies being regulated {#independence-from-the-companies-being-regulated}

The UK's Competition and Markets Authority warned in 2024 that powerful incumbents could shape AI markets to protect and extend their own positions [[30]](#reference-30). I worry about _regulatory capture_ in that setting: companies gaining enough influence over the people writing and enforcing the rules that those rules begin to serve the companies' commercial interests.

Requirements whose compliance costs only the largest firms can absorb deserve particular scrutiny. A rule that imposes the same costly process on a narrowly limited tool and an agent running someone's accounts would need a very good justification. I want smaller providers to have a way to compete by offering tools with less access and fewer powers.

Regulators need their own technical staff and the resources to inspect the evidence behind a company's claims. Industry advisers should disclose their financial interests, and independent researchers should have opportunities to challenge the companies' claims. The people who will live with a system's consequences should also have a say in whether its risks are acceptable. I want those decisions made by public institutions we can hold accountable, with company executives contributing their expertise as part of a process they do not control.

## Frequently asked questions {#frequently-asked-questions}

If you have come straight here, my main concern is an AI assistant with broad, continuing access to your private accounts and permission to act through them. That arrangement puts your information, and other people's confidences, within its reach.

### My friend works at an AI company and thinks you are overreacting {#my-friend-works-at-an-ai-company-and-thinks-you-are-overreacting}

I would ask which protections your friend is relying on and what they prevent. Someone who works on those protections may have a valuable explanation. Employment alone gives me less reassurance, particularly when the question concerns another team's work or decisions made above them.

Their judgment may also be influenced by a salary, colleagues, and work they care about. When the people they spend most of their day with agree about which risks are acceptable, those assumptions can start to feel like common sense. I can take your friend's sincerity seriously while questioning those incentives. Speaking against an employer can carry costs too: current and former AI-company employees described confidentiality restrictions and fear of retaliation in their 2024 _Right to Warn_ letter [[31]](#reference-31). I would want evidence about the particular product, and scrutiny independent of the company.

### Why aren't people's bank accounts being emptied? {#why-aren-t-people-s-bank-accounts-being-emptied}

Banks put authentication checks, transaction limits, and fraud monitoring between a request and a payment [[32]](#reference-32). An assistant reading a statement may have no authority to move the money. Those controls can also obstruct an attacker trying to use the assistant's access to make a payment.

I would not expect a large provider to want to empty your account. My concern includes what it might learn about you and how it might use that knowledge to influence you. An unauthorized withdrawal gives you something to notice and dispute. That creates complaints, demands for a remedy, and pressure to fix the failure. A company quietly keeping a private fact or using it to influence you may face far less of that pressure, because you have no reason to complain about something you never knew happened. [Remediation requires knowing when things went wrong](#remediation-requires-knowing-when-things-went-wrong) explains why a disclosure can leave you without a warning.

### But I have used these tools and nothing bad happened {#but-i-have-used-these-tools-and-nothing-bad-happened}

If the assistant has reliably completed your tasks, that is evidence of its usefulness. The difficulty is knowing what else you would have noticed. It can finish the job you gave it while a private detail is retained or passed on elsewhere. Your experience gives you less information about those possibilities than about the quality of the answers you have read.

[Remediation requires knowing when things went wrong](#remediation-requires-knowing-when-things-went-wrong) develops this detection problem. You can decide to reduce your exposure without concluding that your past use caused harm.

### Isn't it already too late? {#isn-t-it-already-too-late}

I don't think so. Your life keeps changing: new relationships, worries, plans, and financial circumstances. An old record of you can remain dangerous, but continuing access helps keep it up to date. Stopping those updates limits what someone can learn about the person you are becoming, including what they might use to manipulate you. [Putting the pieces together changes the picture](#putting-the-pieces-together-changes-the-picture) develops that argument.

You cannot reliably call back a secret once it has been copied. I would still disconnect a service you no longer want collecting your information, then ask it to delete the records it holds. Those steps serve different purposes: disconnection stops future access; deletion can reduce what the company retains, though it cannot retrieve every copy already passed on. [Stop supplying what you do not need to supply](#stop-supplying-what-you-do-not-need-to-supply) explains where to start.

### Are you anti-AI? {#are-you-anti-ai}

No. I object to giving an assistant broad access without a convincing reason, and to making people accept that access as a condition of working or studying. I want each proposed use to justify what it asks us to give up. For an assistant seeking access to your accounts, [The access needs a justification](#the-access-needs-a-justification) asks what the task requires and whether the benefit is worth granting that access.

I see promise in scientific discovery and value in help with particular tasks. I also have serious reservations about how these systems use people's work and what they could do to education. Those deserve their own arguments. I have concentrated here on the privacy and security decisions being put in front of you.

### Why should I care about privacy if I have nothing to hide? {#why-should-i-care-about-privacy-if-i-have-nothing-to-hide}

If you were leaving an abusive partner, your new address could put you in danger without revealing any wrongdoing. [Who else could use this against you?](#who-else-could-use-this-against-you) considers other ways these records could be used against you, including by future authorities you might have good reason to fear.

Your records also contain other people's private lives. A friend who confides in you may have reasons for secrecy that you do not know about. [Was that yours to share?](#was-that-yours-to-share) explains why they deserve a say in what you share.

### Can a chat webpage read everything on my computer? {#can-a-chat-webpage-read-everything-on-my-computer}

In normal operation, an ordinary chat webpage has no general access to your files. Browsers restrict that access. You usually have to select files or grant permission for a webpage to read them [[33]](#reference-33). The service does receive what you paste or upload, and connecting an account can give it a way to retrieve more.

Installed apps may receive permission to operate your computer, while browser extensions may be able to read signed-in pages. Look at what the particular tool can reach and do. [Broad permissions increase the attack radius](#broad-permissions-increase-the-attack-radius) explains how an attacker can try to use those permissions, and [The access needs a justification](#the-access-needs-a-justification) discusses how narrowly they should be granted.

### What if the company promises not to train on my data? {#what-if-the-company-promises-not-to-train-on-my-data}

I would welcome that commitment, while still wanting to know how long the service keeps your messages and who can access them. It has to process a message to answer you, and it can retain a copy without using it for training. Anthropic, for example, says its Incognito chats are excluded from training but normally retained for 30 days. Enterprise settings can require even longer retention [[34]](#reference-34).

[Stop supplying what you do not need to supply](#stop-supplying-what-you-do-not-need-to-supply) distinguishes stopping future access from requesting deletion of information already supplied.

### Would a local model or read-only access solve this? {#would-a-local-model-or-read-only-access-solve-this}

Running a model entirely on your device can keep your requests from being sent to a model provider. Check that the surrounding app does its work locally too: Ollama, for example, offers cloud features as well as local ones [[35]](#reference-35). A local agent can still damage files if you give it permission to change them.

Read-only access limits changes, but still lets an assistant retrieve private information. If it can send that information elsewhere, your inbox could remain untouched while its contents are disclosed. [Broad permissions increase the attack radius](#broad-permissions-increase-the-attack-radius) and [Misalignment: Nobody has to hack you for something to go wrong](#misalignment-nobody-has-to-hack-you-for-something-to-go-wrong) explain how an attacker or the assistant's own mistaken judgment can turn granted access into harm.

### What if my work or school expects me to use these tools? {#what-if-my-work-or-school-expects-me-to-use-these-tools}

I recognize that refusing can put your job or education at risk. The institution choosing the tool should have to justify the information it asks you to supply and provide a workable alternative where the use would expose private material unnecessarily. That is part of the responsibility I argue for in [Responsibility before deployment](#responsibility-before-deployment).

Where you have discretion, keep your personal accounts off work devices and work records out of your personal AI account. [Keep personal accounts off work devices](#keep-personal-accounts-off-work-devices) explains navigating those boundaries. A colleague, union, or student representative may also help you raise concerns collectively, especially when the decision affects information belonging to many people.

## References {#references}

1. <span id="reference-1"></span> Firefox Security Team. [Protecting Firefox users following the compromise of eMudhra intermediate certificates](https://blog.mozilla.org/security/2026/10/20/protecting-firefox-users-following-the-compromise-of-emudhra-intermediate-certificates/). Mozilla Security Blog. October 2026. Published October 20, 2026; updated October 21; accessed October 24, 2026.

2. <span id="reference-2"></span> The PHP Foundation. [Today's PHP Security Release, and How We're Strengthening PHP Security](https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/). The PHP Foundation. October 2026. Published October 21, 2026; accessed October 25, 2026.

3. <span id="reference-3"></span> Rivest, Ronald L.; Shamir, Adi; Adleman, Leonard. [A Method for Obtaining Digital Signatures and Public-Key Cryptosystems](https://people.csail.mit.edu/rivest/Rsapaper.pdf). Communications of the ACM. vol. 21, no. 2, pp. 120–126, February 1978. DOI: [10.1145/359340.359342](https://doi.org/10.1145/359340.359342).

4. <span id="reference-4"></span> Meta. [Responsible Innovation in AI Glasses & Quest](https://www.meta.com/actions/responsible-innovation/). Accessed October 24, 2026.

5. <span id="reference-5"></span> Staab, Robin; Vero, Mark; Balunović, Mislav; Vechev, Martin. [Beyond Memorization: Violating Privacy via Inference with Large Language Models](https://proceedings.iclr.cc/paper_files/paper/2024/file/9028b8a3ca98f58e373f0c1497a17448-Paper-Conference.pdf). The Twelfth International Conference on Learning Representations. 2024.

6. <span id="reference-6"></span> Federal Bureau of Investigation. [Criminals Use Generative Artificial Intelligence to Facilitate Financial Fraud](https://www.ic3.gov/psa/2024/psa241203). Internet Crime Complaint Center. December 2024. Public service announcement I-120324-PSA, December 3, 2024; accessed October 25, 2026.

7. <span id="reference-7"></span> Federal Trade Commission. [Scammers use AI to enhance their family emergency schemes](https://consumer.ftc.gov/consumer-alerts/2023/03/scammers-use-ai-enhance-their-family-emergency-schemes). FTC Consumer Advice. March 2023. Accessed October 25, 2026.

8. <span id="reference-8"></span> Chismon, Dave. [Prompt injection is not SQL injection (it may be worse)](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection). UK National Cyber Security Centre. December 2025. Published December 8, 2025; accessed October 24, 2026.

9. <span id="reference-9"></span> Sheasha, Tarek. [How We Built Safety Into Muse](https://research.meta.ai/blog/security-and-safety-for-ai-agents-our-approach-with-muse). Meta AI Research. September 2026. Published September 8, 2026; accessed October 24, 2026.

10. <span id="reference-10"></span> Meier, Dominik; Wahle, Jan Philip; Röttger, Paul; Ruas, Terry; Gipp, Bela. [TrojanStego: Your Language Model Can Secretly Be a Steganographic Privacy Leaking Agent](https://aclanthology.org/2025.emnlp-main.1386/). Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing. Association for Computational Linguistics. pp. 27244–27261, November 2025. DOI: [10.18653/v1/2025.emnlp-main.1386](https://doi.org/10.18653/v1/2025.emnlp-main.1386).

11. <span id="reference-11"></span> Grantham-Philips, Wyatte. [AI agents are only as good as the personal information you share. That raises privacy concerns](https://www.ap.org/news-highlights/spotlights/2026/ai-agents-are-only-as-good-as-the-personal-information-you-share-that-raises-privacy-concerns/). The Associated Press. October 2026. Published October 19, 2026; accessed October 24, 2026.

12. <span id="reference-12"></span> Meta. [Introducing Muse: The World's First Personal AI Agent Built for Everyone](https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/). Meta Newsroom. September 2026. Published September 8, 2026; accessed October 24, 2026.

13. <span id="reference-13"></span> Bostrom, Nick. [Ethical Issues in Advanced Artificial Intelligence](https://nickbostrom.com/papers/ethical-issues-in-advanced-ai/). Cognitive, Emotive and Ethical Aspects of Decision Making in Humans and in Artificial Intelligence. International Institute of Advanced Studies in Systems Research and Cybernetics. vol. 2, pp. 12–17, 2003. Slightly revised online version; accessed October 25, 2026.

14. <span id="reference-14"></span> Anthropic. [Our framework for developing safe and trustworthy agents](https://www.anthropic.com/news/our-framework-for-developing-safe-and-trustworthy-agents). Anthropic. August 2025. Published August 4, 2025; accessed October 24, 2026.

15. <span id="reference-15"></span> Federal Trade Commission. [FTC Gives Final Approval to Order Banning BetterHelp from Sharing Sensitive Health Data for Advertising, Requiring It to Pay $7.8 Million](https://www.ftc.gov/news-events/news/press-releases/2023/07/ftc-gives-final-approval-order-banning-betterhelp-sharing-sensitive-health-data-advertising). Federal Trade Commission. July 2023. Published July 14, 2023; accessed October 24, 2026.

16. <span id="reference-16"></span> Vargas, Jose Antonio. [The Face of Facebook](https://www.newyorker.com/magazine/2010/09/20/the-face-of-facebook). The New Yorker. September 2010. Published September 13, 2010; accessed October 25, 2026.

17. <span id="reference-17"></span> Slaughter, Rebecca Kelly. [Dissenting Statement of Commissioner Rebecca Kelly Slaughter: In the Matter of FTC vs. Facebook](https://www.ftc.gov/system/files/documents/public_statements/1536918/182_3109_slaughter_statement_on_facebook_7-24-19.pdf). Federal Trade Commission. July 2019. July 24, 2019, especially pp. 8 and 11; accessed October 24, 2026.

18. <span id="reference-18"></span> Federal Trade Commission. [FTC Finalizes Order with X-Mode and Successor Outlogic Prohibiting it from Sharing or Selling Sensitive Location Data](https://www.ftc.gov/news-events/news/press-releases/2024/04/ftc-finalizes-order-x-mode-successor-outlogic-prohibiting-it-sharing-or-selling-sensitive-location). Federal Trade Commission. April 2024. Accessed October 25, 2026.

19. <span id="reference-19"></span> Office of the Director of National Intelligence. [Intelligence Community Policy Framework for Commercially Available Information](https://www.dni.gov/files/ODNI/documents/CAI/Commercially-Available-Information-Framework-May2024.pdf). Office of the Director of National Intelligence. May 2024. Accessed October 24, 2026.

20. <span id="reference-20"></span> Google. [How Google handles government requests for user information](https://policies.google.com/terms/information-requests). Google Privacy & Terms. Accessed October 25, 2026.

21. <span id="reference-21"></span> Kansas Commission on Peace Officers' Standards and Training. [Integrity Bulletin, Volume 21](https://kscpost.gov/wp-content/uploads/integrityjan25.pdf). Kansas Commission on Peace Officers' Standards and Training. January 2025. January 2025, p. 2; accessed October 25, 2026.

22. <span id="reference-22"></span> Nieles, Michael; Dempsey, Kelley; Pillitteri, Victoria Yan. [An Introduction to Information Security](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-12r1.pdf). National Institute of Standards and Technology. NIST Special Publication, 800-12 Rev. 1, June 2017. DOI: [10.6028/NIST.SP.800-12r1](https://doi.org/10.6028/NIST.SP.800-12r1). Especially sections 5.4.3 and 10.1; accessed October 25, 2026.

23. <span id="reference-23"></span> Google. [Manage links between your Google Account & apps from other developers](https://support.google.com/accounts/answer/13533235). Google Account Help. Accessed October 25, 2026.

24. <span id="reference-24"></span> OpenAI. [US Privacy Policy](https://openai.com/policies/privacy-policy/). OpenAI. Privacy rights and requests through the Privacy Portal; accessed October 25, 2026.

25. <span id="reference-25"></span> National Cyber Security Centre. [Top tips for staying secure online: Managing your passwords](https://www.ncsc.gov.uk/collection/top-tips-for-staying-secure-online/password-managers). UK National Cyber Security Centre. Page updated May 21, 2026; accessed October 25, 2026.

26. <span id="reference-26"></span> National Cyber Security Centre. [Passkeys: what you need to know](https://www.ncsc.gov.uk/passkeys). UK National Cyber Security Centre. Accessed October 25, 2026.

27. <span id="reference-27"></span> National Cyber Security Centre. [Top tips for staying secure online: Install the latest software and app updates](https://www.ncsc.gov.uk/collection/top-tips-for-staying-secure-online/install-the-latest-software-and-app-updates). UK National Cyber Security Centre. Accessed October 25, 2026.

28. <span id="reference-28"></span> National Cyber Security Centre. [Mobile device management](https://www.ncsc.govt.nz/protect-your-organisation/mobile-device-management/). New Zealand National Cyber Security Centre. Accessed October 25, 2026.

29. <span id="reference-29"></span> Federal Trade Commission. [A Brief Overview of the Federal Trade Commission's Investigative, Law Enforcement, and Rulemaking Authority](https://www.ftc.gov/about-ftc/mission/enforcement-authority). Federal Trade Commission. July 2025. Revised July 2025; accessed October 25, 2026.

30. <span id="reference-30"></span> Competition and Markets Authority. [CMA outlines growing concerns in markets for AI Foundation Models](https://www.gov.uk/government/news/cma-outlines-growing-concerns-in-markets-for-ai-foundation-models). GOV.UK. April 2024. Published April 11, 2024; accessed October 25, 2026.

31. <span id="reference-31"></span> Hilton, Jacob; Kokotajlo, Daniel; Kumar, Ramana; Nanda, Neel; Saunders, William; Wainwright, Carroll; Ziegler, Daniel; others. [A Right to Warn about Advanced Artificial Intelligence](https://righttowarn.ai/). June 2024. Open letter from current and former AI-company employees, June 4, 2024; accessed October 25, 2026.

32. <span id="reference-32"></span> Federal Financial Institutions Examination Council. [Authentication and Access to Financial Institution Services and Systems](https://www.federalreserve.gov/frrs/guidance/authentication-and-access-to-financial-institution-services-and-systems-interagency-guidance.htm). Interagency Guidance, reproduced in the Federal Reserve Regulatory Service. August 2021. Issued August 11, 2021; accessed October 25, 2026.

33. <span id="reference-33"></span> MDN contributors. [File System API](https://developer.mozilla.org/en-US/docs/Web/API/File_System_API). MDN Web Docs. Accessed October 25, 2026.

34. <span id="reference-34"></span> Anthropic. [Use incognito chats](https://support.claude.com/en/articles/12260368-use-incognito-chats). Claude Help Center. Accessed October 25, 2026.

35. <span id="reference-35"></span> Ollama. [FAQ](https://docs.ollama.com/faq). Ollama documentation. Especially “Does Ollama send my prompts and answers back to ollama.com?” and “How do I disable Ollama's cloud features?”; accessed October 25, 2026.

[^1]: The title is inspired by the color code of [Jeff Cooper](https://en.wikipedia.org/wiki/Jeff_Cooper), a U.S. Marine Corps officer who served in World War II.
[^2]: In the week ending October 24, 2026, when this was written, the [PHP Foundation described two critical flaws](https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/) that could let an attacker run code on an affected web server without logging in, potentially exposing or altering its data [[2]](#reference-2). Separately, [Mozilla explained the eMudhra certificate-key compromise](https://blog.mozilla.org/security/2026/10/20/protecting-firefox-users-following-the-compromise-of-emudhra-intermediate-certificates/): an attacker able to intercept a connection could use fraudulent security certificates to impersonate a website and potentially read or alter its traffic [[1]](#reference-1).
[^3]: The analogy is imperfect: a physical key can also be copied without your knowledge. Nor do you have to choose between a key and a code. Requiring both adds a layer of protection, an example of _defense in depth_. Combining something you have with something you know is also the principle behind two-factor authentication, which we will return to later.
[^4]: Hiding one message inside another is an old idea in computer science. Seeing it done through a useful, readable answer can still feel like science fiction.
[^5]: Meta describes permission checks, restrictions on access, and approval requirements for Muse. It also acknowledges mistakes and attacks through the data the agent reads [[9]](#reference-9).
[^6]: If you haven't come across the paperclip maximizer, I encourage you to read about it [[13]](#reference-13).
[^7]: The FTC finalized a settlement in 2023 barring BetterHelp from sharing health data for advertising [[15]](#reference-15).
[^8]: This example is hypothetical. Meta says Muse does not share conversations or data in its virtual machine with Meta's advertising systems [[9]](#reference-9).
[^9]: Zuckerberg told _The New Yorker_ in 2010 that he regretted saying this.
[^10]: The FTC finalized an order in April 2024 prohibiting the companies from selling or sharing sensitive location data.
[^11]: The framework also calls for safeguards, including legal review and privacy assessments.
[^12]: The case appears in Kansas's January 2025 police-certification bulletin. The officer used Flock to search her new boyfriend's plate another 64 times. His certification was revoked.
[^13]: The documented examples here concern commercial information and vehicle records. These sources do not establish a transfer of Muse data to those systems.
[^14]: The related principle of _least privilege_ limits a program to the permissions it needs for its task [[22]](#reference-22).
[^15]: Its coverage has exceptions, and financial penalties and consumer redress depend on the particular legal route involved [[29]](#reference-29).

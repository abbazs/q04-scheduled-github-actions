# Q04: Create a Scheduled GitHub Action

> **Marks:** 1.0

---

## Question

4 Create a Scheduled GitHub Action (1 mark) 

### Ask AI

  - [What is cron syntax and how do I read '0 * * * *'?](https://www.perplexity.ai/search?q=What%20is%20cron%20syntax%20and%20how%20do%20I%20read%20'0%20*%20*%20*%20*'%3F)
  - [Why use GitHub Actions for scheduling instead of cron on a server?](https://www.perplexity.ai/search?q=Why%20use%20GitHub%20Actions%20for%20scheduling%20instead%20of%20cron%20on%20a%20server%3F)
  - [What are the limitations of GitHub Actions scheduled workflows?](https://www.perplexity.ai/search?q=What%20are%20the%20limitations%20of%20GitHub%20Actions%20scheduled%20workflows%3F)
  - [How do I test a scheduled workflow without waiting for the cron time?](https://www.perplexity.ai/search?q=How%20do%20I%20test%20a%20scheduled%20workflow%20without%20waiting%20for%20the%20cron%20time%3F)
  - [What happens to scheduled workflows if my repository becomes inactive?](https://www.perplexity.ai/search?q=What%20happens%20to%20scheduled%20workflows%20if%20my%20repository%20becomes%20inactive%3F)
  - [How do I make my scheduled workflow commit changes back to the repo?](https://www.perplexity.ai/search?q=How%20do%20I%20make%20my%20scheduled%20workflow%20commit%20changes%20back%20to%20the%20repo%3F)
  - [What is the difference between Cron jobs and Systemd timers in Linux?](https://www.perplexity.ai/search?q=What%20is%20the%20difference%20between%20Cron%20jobs%20and%20Systemd%20timers%20in%20Linux%3F)

## Automating Repository Updates for DevSync

**DevSync Solutions** is a mid-sized software development company specializing in collaborative tools for remote teams. With a growing client base and an expanding portfolio of projects, DevSync emphasizes efficient workflow management and robust version control practices to maintain high-quality software delivery. 

As part of their commitment to maintaining seamless and transparent development processes, DevSync has identified the need to implement automated daily updates to their GitHub repositories. These updates serve multiple purposes: 

  1. **Activity Tracking:** Ensuring that each repository reflects daily activity helps in monitoring project progress and team engagement. 
  2. **Automated Documentation:** Regular commits can be used to update status files, logs, or documentation without manual intervention. 
  3. **Backup and Recovery:** Automated commits provide an additional layer of backup, ensuring that changes are consistently recorded. 
  4. **Compliance and Auditing:** Maintaining a clear commit history aids in compliance with industry standards and facilitates auditing processes. 

Manually managing these daily commits is inefficient and prone to human error, especially as the number of repositories grows. To address this, DevSync seeks to automate the process using GitHub Actions, ensuring consistency, reliability, and scalability across all projects. 

DevSync's DevOps team has decided to standardize the implementation of GitHub Actions across all company repositories. The objective is to create a scheduled workflow that runs once daily, adds a commit to the repository, and ensures that these actions are consistently tracked and verifiable. 

As a junior developer or DevOps engineer at DevSync, you are tasked with setting up this automation for a specific repository. This exercise will not only enhance your understanding of GitHub Actions but also contribute to the company's streamlined workflow management. 

## Your Task

Create a scheduled [GitHub action](https://github.com/features/actions) that runs daily and adds a commit to your repository. The workflow should: 

  - Use `schedule` with `cron` syntax to run **once per day** (must use specific hours/minutes, not wildcards) 
  - Include a step with your email `22f2000997@ds.study.iitm.ac.in` in its name
  - Create a commit in each run
  - Be located in `.github/workflows/` directory

After creating the workflow:

  - Trigger the workflow and wait for it to complete
  - Ensure it appears as the **most recent action** in your repository
  - Verify that it creates a commit during or within 5 minutes of the workflow run

Enter your repository URL (format: `https://github.com/USER/REPO`): 

Correct!

Incorrect. Try again.

[Discuss](https://github.com/sanand0/tools-in-data-science-public/discussions/208) [__Ask AI](https://www.perplexity.ai/search?q=Write%20an%20ELI15%20step-by-step%20solution%20to%20this%20assignment%20question%20for%20a%20complete%20novice.%0A%0A---%0A%0A4%20Create%20a%20Scheduled%20GitHub%20Action%20\(1%20mark\)%20%0A%0A%23%23%23%20Ask%20AI%0A%0A-%20%5BWhat%20is%20cron%20syntax%20and%20how%20do%20I%20read%20'0%20%5C*%20%5C*%20%5C*%20%5C*'%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DWhat%2520is%2520cron%2520syntax%2520and%2520how%2520do%2520I%2520read%2520'0%2520%252A%2520%252A%2520%252A%2520%252A'%253F\)%0A-%20%5BWhy%20use%20GitHub%20Actions%20for%20scheduling%20instead%20of%20cron%20on%20a%20server%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DWhy%2520use%2520GitHub%2520Actions%2520for%2520scheduling%2520instead%2520of%2520cron%2520on%2520a%2520server%253F\)%0A-%20%5BWhat%20are%20the%20limitations%20of%20GitHub%20Actions%20scheduled%20workflows%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DWhat%2520are%2520the%2520limitations%2520of%2520GitHub%2520Actions%2520scheduled%2520workflows%253F\)%0A-%20%5BHow%20do%20I%20test%20a%20scheduled%20workflow%20without%20waiting%20for%20the%20cron%20time%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DHow%2520do%2520I%2520test%2520a%2520scheduled%2520workflow%2520without%2520waiting%2520for%2520the%2520cron%2520time%253F\)%0A-%20%5BWhat%20happens%20to%20scheduled%20workflows%20if%20my%20repository%20becomes%20inactive%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DWhat%2520happens%2520to%2520scheduled%2520workflows%2520if%2520my%2520repository%2520becomes%2520inactive%253F\)%0A-%20%5BHow%20do%20I%20make%20my%20scheduled%20workflow%20commit%20changes%20back%20to%20the%20repo%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DHow%2520do%2520I%2520make%2520my%2520scheduled%2520workflow%2520commit%2520changes%2520back%2520to%2520the%2520repo%253F\)%0A-%20%5BWhat%20is%20the%20difference%20between%20Cron%20jobs%20and%20Systemd%20timers%20in%20Linux%3F%5D\(https%3A%2F%2Fwww.perplexity.ai%2Fsearch%3Fq%3DWhat%2520is%2520the%2520difference%2520between%2520Cron%2520jobs%2520and%2520Systemd%2520timers%2520in%2520Linux%253F\)%0A%0A%23%23%20Automating%20Repository%20Updates%20for%20DevSync%0A%0A**DevSync%20Solutions**%20is%20a%20mid-sized%20software%20development%20company%20specializing%20in%20collaborative%20tools%20for%20remote%20teams.%20With%20a%20growing%20client%20base%20and%20an%20expanding%20portfolio%20of%20projects%2C%20DevSync%20emphasizes%20efficient%20workflow%20management%20and%20robust%20version%20control%20practices%20to%20maintain%20high-quality%20software%20delivery.%20%0A%0AAs%20part%20of%20their%20commitment%20to%20maintaining%20seamless%20and%20transparent%20development%20processes%2C%20DevSync%20has%20identified%20the%20need%20to%20implement%20automated%20daily%20updates%20to%20their%20GitHub%20repositories.%20These%20updates%20serve%20multiple%20purposes%3A%20%0A%0A1.%20**Activity%20Tracking%3A**%20Ensuring%20that%20each%20repository%20reflects%20daily%20activity%20helps%20in%20monitoring%20project%20progress%20and%20team%20engagement.%0A2.%20**Automated%20Documentation%3A**%20Regular%20commits%20can%20be%20used%20to%20update%20status%20files%2C%20logs%2C%20or%20documentation%20without%20manual%20intervention.%0A3.%20**Backup%20and%20Recovery%3A**%20Automated%20commits%20provide%20an%20additional%20layer%20of%20backup%2C%20ensuring%20that%20changes%20are%20consistently%20recorded.%0A4.%20**Compliance%20and%20Auditing%3A**%20Maintaining%20a%20clear%20commit%20history%20aids%20in%20compliance%20with%20industry%20standards%20and%20facilitates%20auditing%20processes.%0A%0AManually%20managing%20these%20daily%20commits%20is%20inefficient%20and%20prone%20to%20human%20error%2C%20especially%20as%20the%20number%20of%20repositories%20grows.%20To%20address%20this%2C%20DevSync%20seeks%20to%20automate%20the%20process%20using%20GitHub%20Actions%2C%20ensuring%20consistency%2C%20reliability%2C%20and%20scalability%20across%20all%20projects.%20%0A%0ADevSync's%20DevOps%20team%20has%20decided%20to%20standardize%20the%20implementation%20of%20GitHub%20Actions%20across%20all%20company%20repositories.%20The%20objective%20is%20to%20create%20a%20scheduled%20workflow%20that%20runs%20once%20daily%2C%20adds%20a%20commit%20to%20the%20repository%2C%20and%20ensures%20that%20these%20actions%20are%20consistently%20tracked%20and%20verifiable.%20%0A%0AAs%20a%20junior%20developer%20or%20DevOps%20engineer%20at%20DevSync%2C%20you%20are%20tasked%20with%20setting%20up%20this%20automation%20for%20a%20specific%20repository.%20This%20exercise%20will%20not%20only%20enhance%20your%20understanding%20of%20GitHub%20Actions%20but%20also%20contribute%20to%20the%20company's%20streamlined%20workflow%20management.%20%0A%0A%23%23%20Your%20Task%0A%0ACreate%20a%20scheduled%20%5BGitHub%20action%5D\(https%3A%2F%2Fgithub.com%2Ffeatures%2Factions\)%20that%20runs%20daily%20and%20adds%20a%20commit%20to%20your%20repository.%20The%20workflow%20should%3A%20%0A%0A-%20Use%20%60schedule%60%20with%20%60cron%60%20syntax%20to%20run%20**once%20per%20day**%20\(must%20use%20specific%20hours%2Fminutes%2C%20not%20wildcards\)%0A-%20Include%20a%20step%20with%20your%20email%20%6022f2000997%40ds.study.iitm.ac.in%60%20in%20its%20name%0A-%20Create%20a%20commit%20in%20each%20run%0A-%20Be%20located%20in%20%60.github%2Fworkflows%2F%60%20directory%0A%0AAfter%20creating%20the%20workflow%3A%0A%0A-%20Trigger%20the%20workflow%20and%20wait%20for%20it%20to%20complete%0A-%20Ensure%20it%20appears%20as%20the%20**most%20recent%20action**%20in%20your%20repository%0A-%20Verify%20that%20it%20creates%20a%20commit%20during%20or%20within%205%20minutes%20of%20the%20workflow%20run%0A%0AEnter%20your%20repository%20URL%20\(format%3A%20%60https%3A%2F%2Fgithub.com%2FUSER%2FREPO%60\)%3A)

---

## Useful Links
- [TDS Public Discussions](https://github.com/sanand0/tools-in-data-science-public/discussions/)
- [AI Pipe](https://aipipe.org/) — LLM API proxy used in the exam

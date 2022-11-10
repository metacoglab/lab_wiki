---
layout: default
title: Running Online Experiments
rank: 7
---


### Before testing

**Note that all online experiments require ethics - do not collect data without first discussing this with Steve**

1. Decide whether you would like to program your experiment in Gorilla (which has a point-and-click “task builder” but is less flexible than javascript) or javascript / jsPsych (we have a couple of javascript tasks hosted on Gorilla which could be reused on this platform). Eoin Travers has written an [excellent blog post](http://www.eointravers.com/post/web-2/) about the pros and cons of both options. 
2. Program your experiment and upload it to the server (Gorilla will automatically take care of this for you if you are using it), and make sure you can collect data on yourself / friends / lab members via a browser link before moving forward to recruitment.
3. Decide where to recruit from: UCL SONA, Prolific or Amazon Mechanical Turk. We find that Prolific gives reliable data, but that MTurk might be more diverse for certain questions (e.g. individual differences in mental health, political attitudes, etc). If you use Prolific, use the lab Prolific account, rather than creating your own Prolific account.

### Hosting your task on Gorilla

1. Make an account on Gorilla using your UCL email address
2. Email pals.gorilla@ucl.ac.uk to ask to be added to the institutional subscription (mention that you are a student/postdoc in the MetaLab supervised by Prof. Stephen Fleming)
3. Request the number of participant tokens you are going to need for your study
4. On the “recruitment” tab, select “Change Recruitment Policy” -> Recruitment Service -> Select relevant option (eg Prolific, SONA…). 

### Hosting your experiments on MindProbe

1. Install a [local JATOS instance](https://www.jatos.org/Installation.html) on your computer and [familiarize yourself with it](http://www.jatos.org/Get-started.html).
2. Code your experiment so that it runs on your browser. A good way to start is by downloading an example study from the [JATOS gallery](https://www.jatos.org/Example-Studies.html), get it to work on your machine, and then slowly adapt it until it matches the experiment that you had in mind. An alternative is to start with our [MetaLab online study template](https://github.com/metacoglab/lab_wiki/blob/master/metalab_experiment_template.jzip), which already includes the lab’s information sheet and consent form. Good resources on how to build online experiments are Eoin Travers’ blog posts 3 and 4.
3. Don’t forget to add the necessary information sheet and informed consent pages as the first components of your experiment. The latest versions can be found in the lab’s Dropbox.
4. Deploy the study to the remote server, following the instructions [here](https://www.jatos.org/Deploy-to-a-server-installation.html). We use MindProbe: a free server for online experiments. This means that all of the data collected from your participants in prolific will be stored on MindProbe’s server, until downloaded to your local storage. To access the server, you will first need to create an account (follow the steps described here: https://mindprobe.eu/). You can then log into JATOS from mindprobe.eu with your assigned credentials. If you use Gorilla, they will take care of hosting your experiment for you.
5. In the remote server, make the necessary adaptations according to whether you are recruiting from Prolific or MTurk.
6. Start a new batch for your experiment and enable the ‘General Multiple Worker’ option in the batch manager. This link can now be used to recruit participants for your study!

### Recruiting from Prolific

1. Sign into the lab Prolific account (ask Steve for the login details)  	
2. Click on ‘New project’ and add the details. Label your project in an easy-to-read manner (the “project name” field), with format Surname_Project_MonthYear e.g. Fleming_ConfidenceTask_Jan2020. 
3. Target £7.50 per hour for each subject inclusive of bonus (if you need the account topping up message Steve on the #online_recruitment Slack channel with the expected number of subjects you are planning to test)
4. Participants can be paid their bonus manually (by selecting the participant id and clicking Bonus Payment) or in a batch, by clicking ‘Bulk Bonus Payment’ under ‘More’ and pasting in the bonus list in csv format: [subj_id, bonus in pounds]. This can be useful if the bonus can be different for different participants.
5. Basic demographic data can be downloaded by clicking ‘Download Export’ under ‘More’. This includes participants’ age, nationality, gender, and time taken to complete the study, among other fields.
6. Prolific allows adding participants to a study in an incremental manner. This is useful for starting small and doing data-quality checks, as well as for avoiding having too many participants performing the study at the same time. It’s often not a bad idea to set the initial required number of participants to be 1, just to see that everything is working properly. Adding new participants can then be done from the study page, under ‘action’>’increase places’.

### Recruiting from UCL Psychology Subject Pool

1. Make a Participant account on [the SONA website](https://uclpsychology.sona-systems.com/Default.aspx?ReturnUrl=%2f) using your UCL email.
2. Email pals.subjectpool@ucl.ac.uk to ask for a Researcher account. Be sure to mention the username you selected for your Participant account, and also explain who you are (e.g., a student/postdoc in the MetaLab supervised by Prof. Stephen Fleming).
3. Once your request is approved, you will receive an email with login details. The PALS SONA email is only monitored one day per week, so account requests will take time to process.
4. When you log in, you will be prompted to choose between logging on as a Participant or as a Researcher -- pick 'Researcher'.
5. Click on ‘Add New Study’, select 'Online External Study' for credit, and add the details.
6. Target 1 credit per hour of participation (0.25, 0.5 and 0.75 credits are possible, e.g. 0.5 credits for 30 minutes of participation). Remember to select 'Yes' for 'Approved?' and 'Active Study?', so that your study will show up on the list of available studies to participants).
7. Once you have added the study, you can add prescreen restrictions such as normal eyesight (Study Menu > View/Modify Restrictions).
8. To recruit participants, add a timeslot (Study Menu > View/Administer Time Slots > Add a Timeslot), select the final participation date and hour, and how many participants you'd like to recruit. You can start with one or two participants to make sure everything is working correctly, and then later recruit additional ones -- either by adding new timeslots, or by modifying existing ones increasing the number of places (Study Menu > View/Administer Time Slots > Modify > Update Timeslot). There is no limit on how many participants you can recruit, but it will take a few days for the slots to fill up.
9. There is a helpful option in SONA to automatically append each participant's SONA id to the study URL, so that you may record ids without asking participants to manually type them in. Simply add "?sona_id=%SURVEY_CODE%" at the end of your Study URL. 
10. You may grant credits automatically by redirecting your participants to SONA at the end of the experiment. Get the completion URL listed on the Study Menu (under Completion URLs, client side), and replace 'XXX' with each participant's SONA id.
11. For more info on integrating SONA and other platforms, see these helpful pages: [SONA and JsPsych](https://www.sona-systems.com/help/jspsych/) or [SONA and Jatos](https://osdoc.cogsci.nl/3.3/manual/osweb/sonasystems/) or [SONA and Gorilla](https://www.sona-systems.com/help/gorillasc/) or [other platforms](https://www.sona-systems.com/help/).

### During data collection

1. Before you actually run the task, give everybody a heads up via our #online_recruitment slack group to make sure you won’t be using funds someone else is expecting to use.
2. Throughout your recruitment period, keep an eye on both the Prolific message box and the Metalab UCL email account. You will get lots of Prolific messages. 
3. It may be that someone messages you saying that they started the experiment but could not get a completion code (what they need to insert in Prolific/MTurk to get paid). It is important to check whether this is actually the case (i.e. whether you have their data) because people may try to get money from you without doing the task. If you are unsure whether a claim is legitimate, err on the side of paying the baseline payment.

### Tips and hints

* A good time to launch data collection is in the morning between 9-11 am (so that you have the rest of the day for participants to submit their responses and be able to process payments on the whole batch at once)
* For large studies, planning on collection N=40 per day is a reasonable number to aim for. To add subjects incrementally in Prolific, click ‘increase places’ on your study page (no need to start a new study for each new batch!). 
* It’s fine to recruit during the weekend if you wish to, although avoid times where people might be logging on after a Friday/Saturday night out! If you run a study at different times of the day, you might find you have people from different parts of the world taking part.
* If you can be present while they are doing your experiment, you can often respond to a message and salvage a participant who would have aborted. You can never reduce the number of participants. This means that if you reject some participants, their places will be recycled. This can lead to you having more participants than you meant to.  If it’s all going badly, instead of increasing the number of participants, it is possible to finish your present experiment and create a new version of the experiment which excludes your previous participants from taking part, meaning you can merge the data sets if all other things are OK.
* **IMPORTANT: Let Steve know about any subject complaints ASAP!**

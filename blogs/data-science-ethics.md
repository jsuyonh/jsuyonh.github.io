---
title: "What a Survey Can Teach Us About Data Science Ethics"
date: 2026-10-25T08:00:00-03:00
draft: false
author: "Maria Elena Vargas"
tags:
  - Data Science Ethics
  - Privacy
  - Data Ethics
description: "An ethical analysis of student surveys, anonymity, privacy, transparency, informed consent, and responsible data science practices."
toc: true
---

# What a Survey Can Teach Us About Data Science Ethics

## Introduction: Can a survey really be anonymous?

As a data analyst, I am hired by an educational institution to process the results of a survey that students are required to complete at the end of a course. Students receive a 10-question survey; to complete it, they must access a specific URL in their web browser—which is available only for a short period—and log in using their organizational username and password.

At the beginning of the survey, the course name is requested, but the participant’s name is not. Meanwhile, the page description states that all responses and the survey itself are anonymous.

The executive leadership team intends to use the survey results to determine which courses need to be redesigned or updated.

As a data analyst, my role is to provide the executive team with actionable insights that will enable them to take further steps.

The first question on the survey is shown here:

The organization has a legitimate objective. However, the fact that a business purpose is useful does not automatically mean that every method used for data collection or analysis is ethical. Therefore, the ethical issue is not merely whether the survey is anonymous, but whether that claim is accurate, understandable, and supported by the underlying system.

In this post, I will provide commentary from the perspective of a data analyst, drawing on the text by Martens, D. (2022), “Data Science Ethics: Concepts, Techniques, and Cautionary Tales”. Their FAT Flow framework considers the various stages of a data project and asks whether the practices are fair, accountable, and transparent.

## 1. Ethical issues

Privacy: Is a component of fairness and that ethical data science requires balancing data utility with ethical concerns and also is a human right. The requirement to log in creates a potential link between a student’s identity and their participation.

Transparency: Informing participants about what information is being collected, why a login is required, whether identifying data is stored alongside the responses, who can access the original responses, and how the results will be presented.

Informed consent: The organization should explain the purpose of the survey and how the results will be used before students decide whether to participate.

The example question also warrants attention: A student might believe that most objectives were met, but that one significant objective was not. The question does not specify which objectives are being evaluated, and different students might interpret the scale in different ways.  An ethical approach to assessment requires selecting questions and indicators that validly represent the aspect intended for evaluation.

## 2. Other ethical issues present in the survey

Re-identification: It may be possible to re-identify participants even after their names have been removed. Eliminating direct identifiers is often insufficient; a combination of attributes or knowledge of the context can reveal an individual’s identity.

Bias: This can affect who responds and how those responses are interpreted. Students who are highly satisfied or highly dissatisfied may be more likely to respond than those with moderate opinions. Students facing language barriers, accessibility needs, limited internet access, or a fear of retaliation may be less likely to participate. Consequently, the responses may not be representative of the entire class.

Data minimization: An organization should collect only the information necessary for its stated purpose. If the goal is to improve courses, the administration may need feedback on each course, but it likely does not require individual identities, detailed login histories, or unnecessary demographic information.

Purpose limitation and the progressive expansion of data uses: Students are informed that the survey will help identify courses in need of updates. The organization should not quietly repurpose these responses for unrelated objectives—such as penalizing individual instructors, making decisions about specific students, or profiling students' attitudes.

Data security and access controls: The institution should determine who has access to the raw data, whether such access is logged, and when records are deleted. A promise alone does not protect privacy; technical and organizational measures are required.

Finally, there is a risk of misleading interpretations and unintended consequences. If management publishes rankings without context, the results could damage reputations or incentivize instructors to prioritize popularity over learning. Decisions based on weak evidence could lead to unnecessary redesigns or fail to identify courses that are truly in need of improvement.

## 3. Recommendations for executive management

Verify the claim of anonymity before collecting responses. If identity data and responses are stored separately, this should be confirmed and documented. If the system allows them to be linked, the survey should not be described as anonymous; it should either be redesigned to prevent such linking or correctly labeled as "confidential," with clear access restrictions.

Explain the process in plain language. Before the first question, students should be provided with a brief privacy notice explaining the survey’s purpose, what data is being collected, whether login information is kept separate from responses, who has access to the raw data, how the results will be used, how long the data will be retained, and whom to contact with questions. It should also state whether participation is voluntary and whether there are any consequences for declining to respond.

Implement data minimization and privacy-preserving preprocessing. Remove direct identifiers from the dataset whenever possible, limit or avoid the collection of unnecessary metadata, and suppress or aggregate results for very small groups. Free-text comments should be reviewed to remove identifying details before they are shared.

Improve the survey. Replace or supplement general questions with clear, specific questions linked to defined learning objectives. A space for comments can provide context, but students should be advised not to include identifying or sensitive information.

Establish governance and accountability. Assign clear responsibilities for survey administration, privacy protection, data access, analysis, and the approval of reports. Limit access to raw data to authorized personnel, use secure storage and transmission methods, log access, and establish a schedule for data retention and deletion.

Present results responsibly. Display aggregated results, explain limitations, and avoid making unsubstantiated claims about individual students or instructors.

## 4. What options are available to me to act ethically if my recommendations are rejected?

I can still act responsibly within my role by taking the following steps:

I would document the specific concern, the available evidence, the uncertainties, and the potential consequences. I would distinguish confirmed facts from mere possibilities. For example, I would not claim that the survey definitively identifies students unless the system’s design proves it does. Instead, I would explain that the login requirement raises an issue that must be verified before an absolute guarantee of anonymity can be justified.

I would present management with a concise assessment of risks and practical alternatives—such as decoupling authentication from response storage, restricting access to raw data, aggregating results, or revising the privacy notice.

I would seek guidance through the appropriate internal channels, such as the privacy officer, the information security team, an ethics committee, the instructor in charge of the course, or another designated governance body.

I would refuse to include unsubstantiated claims in my analysis or report. I would provide an honest account of the limitations and recommend that the findings be treated with caution until the issue is resolved.

Finally, I would consider formally escalating the matter in accordance with institutional policies and applicable professional obligations. I would not access student records without authorization, publicly disclose confidential information, or alter results to force a desired conclusion. Acting ethically means raising concerns through appropriate channels, protecting the individuals affected, and maintaining the integrity of the analysis. If asked to participate in deception or the misuse of data, I would seek proper guidance and refuse to carry out any specific action that conflicts with my professional responsibilities.

Scientists and data analysts make decisions regarding data, methods, interpretation, and communication. Even if a manager approves a project, the analyst remains responsible for honestly explaining what the evidence can—and cannot—demonstrate.

## Conclusion: Reliable data requires reliable practices.

"Anonymous" is not just a label to be affixed to a form; it is a property that must be designed, verified, and maintained with integrity. Examining the project through the FAT Flow framework revealed issues regarding fairness in privacy, a lack of transparency, and unclear accountability—from data collection through to reporting. The best data scientists do not merely ask, "Can we do this?" but rather, "Should we, and how?" Answering this second question is what transforms a number on a scale from 0 to 10 into a decision that people can trust.

Ethical data science is not simply about gathering enough information to decide; it is about making decisions in a way that respects the individuals represented by that data.

# Threat Hunting Techniques and Pseudocode
<b>Overview : </b><br>
This repository contains a comprehensive collection of threat hunting techniques and their corresponding pseudocode or implementation examples, organized by various adversary groups. The information provided here is designed to help threat hunters enhance their hunting capabilities by leveraging structured techniques mapped to the MITRE ATT&CK framework.

Threat hunters can use these techniques for both conditional and hypothesis-based hunting, allowing for proactive detection and mitigation of adversarial behaviors within their environment.

<b> How This Helps Threat Hunters :  </b><br>
Threat hunting is the process of actively searching for signs of malicious activity within an organization's infrastructure. It's a proactive approach to cybersecurity, where threat hunters go beyond automated defenses like SIEM systems to manually search for indicators of compromise (IoCs), anomalous behaviors, and potential threats.

<b>This repository provides valuable resources for threat hunters by: </b><br>

<b>Organizing Techniques by Adversary Groups:  </b><br>

Each adversary group has a dedicated file with the techniques they commonly use. This allows threat hunters to focus on specific groups that may pose a threat to their environment.
Knowing the techniques used by certain threat actors helps hunters understand what tactics and procedures (TTPs) are likely to be employed by the adversary, enabling them to be more focused and effective in their investigations.

<b>Providing Pseudocode for Detection:</b> <br>

The repository includes pseudocode or implementations for detecting the techniques in action. This can be directly utilized or adapted to fit into existing threat detection tools and processes.
Hunters can take this pseudocode and apply it within their SIEM platforms, EDR tools, or even create custom detection rules in scripting environments. The pseudocode helps threat hunters quickly deploy detection mechanisms without having to start from scratch.

<b>Mapping to Kill Chain Phases:</b><br>

Each technique is accompanied by its associated kill chain phases. This allows hunters to understand which part of the attack lifecycle the technique belongs to (e.g., initial access, execution, persistence, lateral movement, etc.).
By mapping techniques to the kill chain, hunters can effectively hunt for threats at various stages of an attack and take preemptive measures at key points in the lifecycle.
Supporting Conditional and Hypothesis-Based Hunting:

<b> Conditional Threat Hunting: </b><br>

This approach is driven by known indicators of compromise (IoCs) and well-documented patterns of behavior. Hunters can take the techniques and pseudocode provided here to look for specific behaviors that are known to indicate malicious activity.
For example, if an organization knows they are a target of a particular adversary group (e.g., APT29), they can directly search for techniques employed by that group using the pseudocode provided.
Conditional hunting is useful when a clear trail is present (e.g., from previous incidents or threat intelligence feeds) and the hunter can follow up on specific conditions that lead to the identification of a threat.

<b> Hypothesis-Based Hunting: </b><br>

In contrast to conditional hunting, hypothesis-based hunting involves creating assumptions about how adversaries might behave in the environment. Hunters begin by hypothesizing potential adversary behaviors and then explore whether there is evidence to support those hypotheses.
This repository aids hypothesis-based hunting by offering a catalog of techniques across multiple adversary groups. A hunter can develop a hypothesis about what an adversary might do in their environment (e.g., using stolen credentials for lateral movement) and then use the corresponding pseudocode to hunt for evidence supporting that hypothesis.
By employing the techniques in this repository, threat hunters can conduct more structured and thorough hypothesis-based investigations, ultimately increasing their chances of detecting sophisticated threats.

<b>How to Use This Repository  </b><br><br>
<b>Browse Adversary Groups:  </b><br>

Each text file in the repository is named after an adversary group. You can begin by identifying a specific group of interest (based on threat intelligence or recent trends) and explore the techniques associated with that group.

<b>Understand the Techniques: </b><br>

Inside each group’s text file, you will find a list of techniques that the adversary group is known to use. Each technique includes:
Technique ID: The unique identifier for the technique.
Kill Chain Phases: The stages of the attack lifecycle where the technique is likely to occur.
Pseudocode: Examples of detection logic for the technique, which can be adapted for use in detection platforms.

<b>Implement Pseudocode in Your Environment: </b><br>

The pseudocode provided can be directly translated into queries for SIEM platforms, EDR tools, or custom threat detection scripts. For example, if you are using a SIEM like Splunk, you can convert the pseudocode into a query in Splunk's Search Processing Language (SPL).
If using endpoint detection tools, you can adapt the logic to query telemetry data and identify suspicious activity.
<b>Customize to Your Environment:</b></br>

The pseudocode is designed to be flexible. Depending on the logs and telemetry available in your environment, you may need to adapt the code to fit your specific use case. The examples provided give you a starting point, but they can be customized to match your network, endpoint configurations, and security stack.
Develop Hypotheses for Threat Hunting:

Use the techniques and their descriptions to form hypotheses about potential adversary activity in your network.
For example, you might hypothesize that an adversary could be using compromised credentials to move laterally. You can then use the pseudocode for techniques related to credential abuse or lateral movement to search for evidence of such activity.
Monitor and Adjust:

Threat hunting is a continuous process. As you uncover evidence of threats or confirm that certain behaviors are benign, refine your hunting techniques. The pseudocode and techniques in this repository can be regularly revisited as your understanding of adversary behaviors evolves.

<b>Benefits of Using This Repository </b><br>

<b>Proactive Threat Detection: </b><br> 
Move beyond reactive alerts and start proactively hunting for potential threats, even when no clear indicators are present.<br>
<b>Hypothesis-Driven Investigations: </b><br>  Develop informed hypotheses about adversary behavior and use the techniques in this repository to validate or disprove your assumptions.<br>
<b>Enhanced Detection Logic: </b><br> Use the provided pseudocode as a starting point for creating custom detection rules and logic in your SIEM or EDR platforms.<br>
<b>Targeted Group-Specific Hunting: </b><br>Focus your efforts on specific adversary groups and their known tactics, techniques, and procedures (TTPs).<br>
Improved Security Posture: By employing proactive and structured threat hunting, your organization will improve its overall security posture, reducing dwell time and increasing the chances of detecting advanced threats.

<b>Conclusion </b><br>

This repository is designed to be a practical tool for both experienced and novice threat hunters. Whether you are conducting conditional-based hunting with known IoCs or engaging in hypothesis-driven investigations, the pseudocode and techniques here will serve as valuable resources for identifying and mitigating threats in your environment. As adversaries evolve, so must your threat hunting techniques—this repository provides a foundation to stay one step ahead.

A detection method that identifies abnormal behaviour
Two phases to anomaly-based analysis: A training phase & a detection phase.
In the training phase a baseline of normal or expected behaviour must be established by collecting data that corresponds to normal system behaviour.
In the detection phase the current system activity is compared against this baseline & activity that's different from the baseline gets logged and an alert is generated.

Advantages:
- Ability to detect new and evolving threats: unlike [[signature-based analysis]], which uses known patterns to detect threats, anomaly based analysis can detect unknown threats.

Disadvantages
- High rate of false positives: Any behaviour that deviates from the baseline can be flagged as abnormal, including non-malicious behaviours, leading to a high rate of false positives.
- Pre-existing compromise: The existence of an attacker during the training phase will include malicious behaviour in the baseline which can lead to missing a pre-existing attacker.

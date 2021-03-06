- Avoid/dis-courage making changes to infrastructure by hand that leads to configuration drift and introduce risks.
- Write your infrastructure as code to enable repeatability, version control, Peer-review of changes/improvements, auditing, preservation of history of Infrastructure evolution.
- Leverage compliance tracking tools like AWS Config to record/track any changes done to the infrastructure. 
- Leverage AWS Cloudtrail to identify the source, destination & time of change.
- Implement an additional mechanism like Replay templates/playbooks to restore the state of infrastructure to what it is defined in the master version.
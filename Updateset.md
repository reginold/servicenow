### When to use Update Set
- Changes you want to keep in every instance
- All the changes which can change the baseline and can give impact
- Changes needs to be tested in Lower instance before moving to Production
### Update Set capture Configuration Items
- Form Configuration, Related List Configuration, Business Rules, Client Script, UI policy, UI actions
- Notification, Script Includes, UI Page
### Update Set capture Configuration Items(exclude)
- Task Records, Users, Groups, Scheduled Jobs, CMDB Records, System Properties, More...
### Update Sets Planning Process
- Dev -> UAT -> Staging -> Prod
### System Update Set Tables
- Update Set[sys_update_set]
- Customer Update[sys_update_xml]
  - CI, list layout, form layout, business rule, 
### Demo
- Create the Remote instance in Update Source.
- Compare the diff in ```updateset compare```.

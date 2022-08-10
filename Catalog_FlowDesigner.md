- [1. Catalog](#1-catalog)
- [2. Flow Designer](#2-flow-designer)
  - [2.1. Ref:](#21-ref)
- [3. Workflow](#3-workflow)
  - [3.1. Workflow and Flow Designer Pro and Con](#31-workflow-and-flow-designer-pro-and-con)
  - [3.2. Develop the workflow](#32-develop-the-workflow)
## 1. Catalog 
- create the catalog item
	- [Youtube: ServiceNow Catalog Item Creation | How to create a catalogue item in ServiceNow](https://www.youtube.com/watch?v=-w49Bu6RpxY&list=PLkXOxVrhArjzQG3-ZkhJ9i_t0t2-jEqkZ)
	- カテゴリ作成
	- アイテム作成
		- item details
		- process engine
	- [Youtube: ServiceNow Flow Designer | Creating a Catalog Item Flow](https://www.google.com/search?q=how+to+create+the+simple+flow+designer+with+service+catalog&rlz=1C1GCEU_jaJP984JP984&oq=how+to+create+the+simple+flow+designer+with+service+catalog&aqs=chrome..69i57j33i160j33i21j33i22i29i30l3.18547j0j4&sourceid=chrome&ie=UTF-8#kpvalbx=_H2bGYq2PKrqw2roPtc6UwAo31)
	- reference: use code or regex positive num
	- show the checkout 観点
		- use yes no and attach the image
- [predictive intelligence](https://docs.servicenow.com/bundle/sandiego-now-intelligence/page/administer/predictive-intelligence/concept/predictive-intelligence.html)
	- just can be used by the incidents problem
- create the catalog variable set
  - You can create the variable set once, and utilize the variable set at other place for recycle.
    - Two kinds of varible set.
      - 1. Single-Row Variable Set.
      - 2. Multi-Row Varibale Set
        - [Multi-Row Variable Sets in ServiceNow | Share the Wealth](https://www.youtube.com/watch?v=SxNcI7-8eaw)
          - The introduction of the multi-row varible sets.
          - Developer can use the X-explore to see the entity of data.
- How to remove OOTB feature:
  - Remove the `<1000` workflow default. 
## 2. Flow Designer
- Error handling
  - Error message showed when create the 
    - ```Flow reports not available. Check flow execution settings. ``` 
  - Fix
    - [Flow reports not available. Check flow execution settings. – フローの詳細(Flow Reports)を確認する (ServiceNow)](https://zw-kakeru.com/tips/servicenow-aes-flow-reports-setting/)

### 2.1. Ref:
- [Platform Academy Session #14 - February 17, 2022 - Flow Designer Good Practices](https://www.youtube.com/watch?v=7LFmisAlrXU)
## 3. Workflow
- Ref: [Success Meetup: Flow Designer vs. Workflows with Steven Bell [Knowledge 2020 ACT2107]](https://www.youtube.com/watch?v=Tp1iQJpNGUs)
- HUGE install base
- with very large trained developer base. In-depth custom development training.
### 3.1. Workflow and Flow Designer Pro and Con
- Very easy to do no-code solutiions in Flow Designer
- Both require serious training to master.
- Workflow has a scratchpad variable
- Workflow has loopback to previous step
- Flow designer has data pills, but cannot expad JSON or non-GlideRecord objects.
- Deployment is the same for both(Update sets, scoped applications) 
- A question about the worfkflow will be taken away --> Answer would be NO. 13:49
### 3.2. Develop the workflow
- [Workflow basic](https://developer.servicenow.com/dev.do#!/learn/courses/quebec/app_store_learnv2_automatingapps_quebec_automating_application_logic/app_store_learnv2_automatingapps_quebec_workflow/app_store_learnv2_automatingapps_quebec_workflow_objectives)
- [Article #9 - Create User Approvals using Catalog Variables](https://community.servicenow.com/community?id=community_article&sys_id=e45144b7dbea9010190b1ea668961963) 
- [How to use a Catalog Item Variable (reference: sys_user) as an Approver in the Workflow Approval Activity.](https://community.servicenow.com/community?id=community_question&sys_id=42eb807ddb1590d05ed4a851ca961946)
- [**Dynamic Approval Configuration** in ServiceNow | Dynamic Approval Workflow ServiceNow](https://www.youtube.com/watch?v=honIwnuiJ7I&t=714s)
- Get the variables from catalog task to email in workflow
  - [Pull catalog item variables into email notification for TASK](https://community.servicenow.com/community?id=community_question&sys_id=5c4503addbd8dbc01dcaf3231f961915)

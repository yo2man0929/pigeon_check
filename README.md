# ecse_pigeon_check
### yicf setting

- YINST set property_name NevecTW
- YINST set yca_role yahoo.nevec.hgp-build

### oldmsgtool

 * list queued information from your property 

> ./pigeon_tool -l

* list queued information from all property

> ./pigeon_tool -l -a

* skip queued message

> ./pigeon_tool -k -q
 CQI.prod.storeeps.set.action::CQO.prod.storeeps.set.action.search.merlin
-m d925d129-e4e7-4602-bba4-124bf462bc5c__08959ef907109ef601

### ymsec_pigeon_oldmsg


     - id: billing_pigeon_old_message
       interval: 300
       check: /home/y/libexec/yms/ymsec_pigeon_oldmsg
       user: ymon
       tags:
           namespace: BillingTW
       args:
         - --property_name=BillingTW
         - --yca_role=yahoo.nevec.hgp-build

### onboard Yams
    Please refer to the link.
    https://git.ouroath.com/ecse/nevectw_yamas2_config/blob/master/rules/pigeon_300.yo
---
[![Build Status](https://api.screwdriver.corp.yahoo.com:4443/badge/310418/component/icon)](https://api.screwdriver.corp.yahoo.com:4443/badge/310418/component/target)

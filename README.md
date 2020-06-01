# Contract Parser

Add support for REST API calls to original [`contract_parser`](https://github.com/agccie/aci-contract-parser). 
All the on-the-apic and offline functionality remains unchanged.

## How to use API version

```
my-linux$  python contract_parser.py --api -u admin -p password --ip apic1

Key:
[prio:RuleId] [vrf:{str}] action protocol src-epg [src-l4] dst-epg [dst-l4] [flags][contract:{str}] [hit=count]

[node:101] [7:4108] [vrf:AutoLab:VRF1] permit ip tn-AutoLab/ap-APP1/epg-EPG1(19) tn-AutoLab/ap-APP1/epg-EPG3(20) [contract:uni/tn-AutoLab/brc-epg1_epg3] [ing:hit=0][egr:hit=0]
[node:101] [7:4110] [vrf:AutoLab:VRF1] permit ip tn-AutoLab/ap-APP1/epg-EPG1(19) tn-AutoLab/ap-APP1/epg-EPG2(49153) [contract:uni/tn-AutoLab/brc-epg1_epg2] [ing:hit=0][egr:hit=0]
```


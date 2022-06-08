Reproduction:
1. Run yarn.

Expect:
* Single react-dom dependency

Output of installed:
```
 % yarn info react-dom -A --virtuals --dependents                        
├─ react-dom@npm:18.1.0
│  ├─ Instances: 2
│  ├─ Version: 18.1.0
│  │
│  └─ Dependencies
│     ├─ loose-envify@npm:^1.1.0 → npm:1.4.0
│     └─ scheduler@npm:^0.22.0 → npm:0.22.0
│
├─ react-dom@npm:18.1.0 [530dc]
│  ├─ Version: 18.1.0
│  │
│  ├─ Dependents
│  │  ├─ package-a@workspace:package-a [0f866]
│  │  └─ package-a@workspace:package-a
│  │
│  └─ Peer dependencies
│     ├─ @types/react@* → ✘
│     └─ react@^18.1.0 → npm:18.1.0
│
└─ react-dom@npm:18.1.0 [753d7]
   ├─ Version: 18.1.0
   │
   ├─ Dependents
   │  ├─ package-b@workspace:package-b [0f866]
   │  └─ package-b@workspace:package-b
   │
   └─ Peer dependencies
      ├─ @types/react@* → npm:18.0.12
      └─ react@^18.1.0 → npm:18.1.0
```

react-dom has 2 instances.

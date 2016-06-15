# verify-trust-paths

Verify trust paths between two gpg keys.

Example: which of `1AE0322EB8F74717BDEABF1D44BB1BA79F6C6333` and
`88BB08F633073D7129383EE71EA37A0C9F6C6333` is the real key?

```
$ ./verify-trust-paths 1793D6AB75663E6BF104953A634F4BD1E7AD5568 1AE0322EB8F74717BDEABF1D44BB1BA79F6C6333
hkt (hopenpgp-tools) 0.18
Copyright (C) 2012-2016  Clint Adams
hkt comes with ABSOLUTELY NO WARRANTY. This is free software, and you are welcome to redistribute it under certain conditions.
(4,[1,4,3,6])

(1,1793D6AB75663E6BF104953A634F4BD1E7AD5568)
(3,F8921D3A7404C86E11352215C7197699B29B232A)
(4,C331BA3F75FB723B5873785B06EAA066E397832F)
(6,1AE0322EB8F74717BDEABF1D44BB1BA79F6C6333)

$ ./verify-trust-paths 1793D6AB75663E6BF104953A634F4BD1E7AD5568 88BB08F633073D7129383EE71EA37A0C9F6C6333
hkt (hopenpgp-tools) 0.18
Copyright (C) 2012-2016  Clint Adams
hkt comes with ABSOLUTELY NO WARRANTY. This is free software, and you are welcome to redistribute it under certain conditions.
(0,[])
```

It requires [hopenpgp-tools](http://floss.scru.org/hopenpgp-tools).

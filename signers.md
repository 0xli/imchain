```
> clique.proposals
{
  0xe64b3a41601f3731b223be1d1235559c823a27fb: false,
  0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: true
}
```
only submit proposal when generate block
```
> clique.getSnapshot()
{
  hash: "0x9e05ca5314010a0b38f69e4f06378bc4ca22624b0f2ca47da79a04e9ec21b7c5",
  number: 1547811,
  recents: {
    1547809: "0x2ce16000864839c035e9343b580d277b88836830",
    1547810: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281",
    1547811: "0xaada53bec20cf15854e357998cae930c89d2a716"
  },
  signers: {
    0x2ce16000864839c035e9343b580d277b88836830: {},
    0xaada53bec20cf15854e357998cae930c89d2a716: {},
    0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281: {},
    0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61: {},
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {}
  },
  tally: {
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {
      authorize: false,
      votes: 1
    },
    0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: {
      authorize: true,
      votes: 2
    }
  },
  votes: [{
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547809,
      signer: "0x2ce16000864839c035e9343b580d277b88836830"
  }, {
      address: "0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1",
      authorize: true,
      block: 1547810,
      signer: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281"
  }, {
      address: "0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1",
      authorize: true,
      block: 1547811,
      signer: "0xaada53bec20cf15854e357998cae930c89d2a716"
  }]
}

```

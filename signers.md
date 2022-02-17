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
add success
```
> clique.getSnapshot()
{
  hash: "0x267935d98b2d752eb1e53e1cb7e8303876b449bbbda3d2d1834ec1ac0d4a2261",
  number: 1547813,
  recents: {
    1547811: "0xaada53bec20cf15854e357998cae930c89d2a716",
    1547812: "0x2ce16000864839c035e9343b580d277b88836830",
    1547813: "0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61"
  },
  signers: {
    0x2ce16000864839c035e9343b580d277b88836830: {},
    0xaada53bec20cf15854e357998cae930c89d2a716: {},
    0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281: {},
    0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61: {},
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {},
    0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: {}
  },
  tally: {
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {
      authorize: false,
      votes: 1
    }
  },
  votes: [{
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547809,
      signer: "0x2ce16000864839c035e9343b580d277b88836830"
  }]
}

```
get one more proposal for remove
```
> clique.getSnapshot()
{
  hash: "0x44ac80b25fce159baeb50696e10acc9d59a86a091bc747e3a47acb597e67ccae",
  number: 1547814,
  recents: {
    1547811: "0xaada53bec20cf15854e357998cae930c89d2a716",
    1547812: "0x2ce16000864839c035e9343b580d277b88836830",
    1547813: "0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61",
    1547814: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281"
  },
  signers: {
    0x2ce16000864839c035e9343b580d277b88836830: {},
    0xaada53bec20cf15854e357998cae930c89d2a716: {},
    0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281: {},
    0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61: {},
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {},
    0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: {}
  },
  tally: {
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {
      authorize: false,
      votes: 2
    }
  },
  votes: [{
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547809,
      signer: "0x2ce16000864839c035e9343b580d277b88836830"
  }, {
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547814,
      signer: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281"
  }]
}

```
need one more to remove
```
> clique.getSnapshot()
{
  hash: "0x20b0dc93730885d9a881f6515282fc84548db8e15c2f230751f4392fb0aa1e33",
  number: 1547815,
  recents: {
    1547812: "0x2ce16000864839c035e9343b580d277b88836830",
    1547813: "0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61",
    1547814: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281",
    1547815: "0xaada53bec20cf15854e357998cae930c89d2a716"
  },
  signers: {
    0x2ce16000864839c035e9343b580d277b88836830: {},
    0xaada53bec20cf15854e357998cae930c89d2a716: {},
    0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281: {},
    0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61: {},
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {},
    0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: {}
  },
  tally: {
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {
      authorize: false,
      votes: 3
    }
  },
  votes: [{
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547809,
      signer: "0x2ce16000864839c035e9343b580d277b88836830"
  }, {
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547814,
      signer: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281"
  }, {
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547815,
      signer: "0xaada53bec20cf15854e357998cae930c89d2a716"
  }]
}
```
this signer not submit proposal
```
> clique.getSnapshot()
{
  hash: "0xa61655fc56ec8d8ed2001ac3f45ad8d5f9926886e67e9fa43e5bd7a17d141093",
  number: 1547816,
  recents: {
    1547813: "0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61",
    1547814: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281",
    1547815: "0xaada53bec20cf15854e357998cae930c89d2a716",
    1547816: "0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1"
  },
  signers: {
    0x2ce16000864839c035e9343b580d277b88836830: {},
    0xaada53bec20cf15854e357998cae930c89d2a716: {},
    0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281: {},
    0xcbb6c355c9ab1ca68aaade61727293cbbd4e6a61: {},
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {},
    0xff9d40c2d790b1737729cd3a4b58c08aead2e7e1: {}
  },
  tally: {
    0xe64b3a41601f3731b223be1d1235559c823a27fb: {
      authorize: false,
      votes: 3
    }
  },
  votes: [{
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547809,
      signer: "0x2ce16000864839c035e9343b580d277b88836830"
  }, {
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547814,
      signer: "0xc1c9e49cd2d7cb1dd204739ecd6ab81f1ff7f281"
  }, {
      address: "0xe64b3a41601f3731b223be1d1235559c823a27fb",
      authorize: false,
      block: 1547815,
      signer: "0xaada53bec20cf15854e357998cae930c89d2a716"
  }]
}

```

# Comparing `tmp/chadplotlib-0.0.1.tar.gz` & `tmp/chadplotlib-0.0.2.tar.gz`

## Comparing `chadplotlib-0.0.1.tar` & `chadplotlib-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,98 @@
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/src/chadplotlib/__init__.py
--rw-r--r--   0        0        0   198120 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Bold.ttf
--rw-r--r--   0        0        0   197756 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Medium.ttf
--rw-r--r--   0        0        0   197624 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Regular.ttf
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/LICENSE
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 chadplotlib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/type
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/2b1e7aa139c18c54257653d8c8b139413cded89df83e31ad939fe0aec4d7ea4eae90427733eb185dfda84c486a3cc9de29ae15192e6c45bfef225d085474239d
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/3f229860e832248f6796b13b0df4a21fbd7fce123418233adb72e6e945ce1699690fdbb8495b5ee457e413755381dfe04cdefcd14b52663751805bf2f9981448
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/475883c27d8be824f7e578fd92a8152e5cf9fd705d2241c48d530e4d17f48066e364a261a6d96b737c956280b0b7aeaca6e4114d2829a8525773a7481740c868
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/5d2da9532d68a2602c8d93a3fe3870808d73f3d217b33859344c787ee80bec43b37bd24d7b4b7a031e92a98bd4650c716043451a13f6e9f07e1af0577e617c62
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/6ff790c336c5631ba758391dbd1710b1e952c76fac4370eed0d3ff9e3e99c581bff4d6e037dc01f0dddbbe795e5798154722356e8d71d680811a17da913f320b
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/7c9d8142d06b93905d660d692120b81eb39e9a17fa2299bb1b2d28164601bb078885228d547d7217e8bbf2da7d22686c3e4f55380957a6b1ae1d809078b8f661
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/a6bbf353f4c4e73431c5498e5b47bdf9970bdc2a24e7ff6ce43a4113e64fcd2b0eb7aba57d922fff0e484feaf9c999c6b3d31d5f36ae215581fb311a0edd667c
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/operations/ea157114c0f05fbea47dd1e4429217acd315d61538994c59feed2dc60decc25763ce0bb3771c7719c0a3d8af65afe4c6f59786af7ff46b5e221d046071ef737a
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/17f9dbdbf054f173de48090c168fbc47c8dd64f9e2bf2283c0e6a50656bb2da1aee604b49f83c7a0820599f67c9a44a771e76a44bfe0a530315ebe6296ba2a4f
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/387f37f9c93868ccdaf2399e133be986823e9a902d2bacef7a40b230ba05b1f6556e91fe63513b93d200abf4ced4026c801171e02ee32e5d563dee685a8f96be
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/44c5b9216851d26e4be8073c838ecf1726b1bf8b7516d42df3b245bb749bc77c69862a0baf334b93ca5814a9e700bd5f609810503414c992ae908f1d67720520
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/945dbeaeaa7445dbea7fe55bb62f1530cba6528bb0a68ff2e0acdf3469081e97ec5b4da1e48fe43fa5f4df5eb2444b9dcdcc26d871364f708a08698da842edca
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/9f28b19a2c2ae5483d37cc57d5e134d62db24f2c39b297e7fbb4d3300bbbc619568ab52938a296e1f4ac76dffa4001342fcbbb468a4d2da157ebbce16f626e29
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/d27ad326963b75736b636adad9fb812eb3f2871e0efb4bc7db37d4b701a4282911eaaee91bed3a759e940769b667be1ed66f2d7f2f41ac3906b87ab7eec19c3a
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/index/segments/d80eaa6cabd204e7d6e0f03501706fd9c0df397376208637a9e0584f60f2ca74fb966efb14453a3cd6703c078518d5d43b796f71bcae1570818e2182520bbfe9
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_heads/type
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_heads/heads/6ff790c336c5631ba758391dbd1710b1e952c76fac4370eed0d3ff9e3e99c581bff4d6e037dc01f0dddbbe795e5798154722356e8d71d680811a17da913f320b
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/type
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/2b1e7aa139c18c54257653d8c8b139413cded89df83e31ad939fe0aec4d7ea4eae90427733eb185dfda84c486a3cc9de29ae15192e6c45bfef225d085474239d
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/3f229860e832248f6796b13b0df4a21fbd7fce123418233adb72e6e945ce1699690fdbb8495b5ee457e413755381dfe04cdefcd14b52663751805bf2f9981448
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/475883c27d8be824f7e578fd92a8152e5cf9fd705d2241c48d530e4d17f48066e364a261a6d96b737c956280b0b7aeaca6e4114d2829a8525773a7481740c868
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/5d2da9532d68a2602c8d93a3fe3870808d73f3d217b33859344c787ee80bec43b37bd24d7b4b7a031e92a98bd4650c716043451a13f6e9f07e1af0577e617c62
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/6ff790c336c5631ba758391dbd1710b1e952c76fac4370eed0d3ff9e3e99c581bff4d6e037dc01f0dddbbe795e5798154722356e8d71d680811a17da913f320b
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/7c9d8142d06b93905d660d692120b81eb39e9a17fa2299bb1b2d28164601bb078885228d547d7217e8bbf2da7d22686c3e4f55380957a6b1ae1d809078b8f661
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/a6bbf353f4c4e73431c5498e5b47bdf9970bdc2a24e7ff6ce43a4113e64fcd2b0eb7aba57d922fff0e484feaf9c999c6b3d31d5f36ae215581fb311a0edd667c
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/operations/ea157114c0f05fbea47dd1e4429217acd315d61538994c59feed2dc60decc25763ce0bb3771c7719c0a3d8af65afe4c6f59786af7ff46b5e221d046071ef737a
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/1c45d739f8d91194ef950f001a928a8bcacbd7c0ce24cb6bc205f9687c8cdba588b2290c826aab8bb9b5f00a913131e487aef21af87d39e10f939b74204e9ddc
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/3a80b98791e09b6d73f2a562609836e528aab951fccc49b15b631bbd44bbbe0ad2d8e4921c35a721c0aacc2d213fd56f2b75334bb0be1b469d2c09b9cf6bcb91
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/5353a337291947250a14803efea62f29ecd92f722fef754501a6fe82c8c49815edf4f757a836115f0486944b00bdffb7a8beb49b829a390c8c0311b1e6f1197c
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/6d7d532d941c82d92279b186fc7b1f256bcf3f1eb3fcfb99ca73ed6d4a918b4f968b0caec808d5bbb668eda6d4b16396f9fd4d012c8da66f9dbb3cc1718a9072
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/7b5368c6e990546fe1454541a1f0ff6dad4508e280e210938a039fafe694a02e78429da29b9f1accfdbe5ba892a666d4c264159629333d5e6f73fd43e330cc14
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/7d1af688e825b0d2bec6797e48bc4bf44301cbf3076c43c9ab2aa96af782364cd61a7cc7c3a0412d62874ff68fcae099ac669ac4c6db8d99689b7a1d02c0697e
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/92b5371bf8ac958dddfcbfe2af524ad2bdf5a69c91543311ef5d3f4b62678dd986aa15c2ee8b9bffb723df15fc1cb7465e7d4c6c6a8247baaff4266c1e6b3d8b
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/op_store/views/b379cf52c815008200fd9040c4df7305018d0575c0202f3d95f64a2cdc74ddab3ef1708158e98782a4248026f677e34b5f8b5e2e3e03a14685cbc07577ae1e3d
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git_target
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/type
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/20b947d3381ffe1648302450c39df525d95a6faca905aa1f962635350a3e7d383befbff046c14d66f6cea2e5e390d8b9554754f1a1c87a3172df8d326f95a8c1
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/41c6343b96d883b362ec55cee2b48a2b5bcd1fd1258ae88140a490f9db570358f2befc4d847b9395e8ed8b640ba2536b1cfa051b5fa81300bac00cdb3e184a75
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/482ae5a29fbe856c7272f2071b8b0f0359ee2d89ff392b8a900643fbd0836eccd067b8bf41909e206c90d45d6e7d8b6686b93ecaee5fe1a9060d87b672101310
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/a7665279aac7b10d8f393d2dbfe57ef3fc9d6d38cfa87cb150f5edd23be5e8f42165a49ccd065e5ea5f3d0a2cd25fdbb4ae82d35552a3e235cb07b3f58697b18
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/a81ba53fcf797bb22785f922a439151ea80449c23a88b7aa5e010b431d23be2fe6ec0754eb3d0239bc586e2fcebc93d8b2ce179311fb008756c0bdbf74141509
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/b0ba50a21f98b3b12ffc11eda80754c838e0888b3298236033629fe0a66f8fe6e4b13fbb78f8795069f5324c5c61860fecaba6e460f7d02572092795ee07cb62
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/extra/heads/a7665279aac7b10d8f393d2dbfe57ef3fc9d6d38cfa87cb150f5edd23be5e8f42165a49ccd065e5ea5f3d0a2cd25fdbb4ae82d35552a3e235cb07b3f58697b18
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/FETCH_HEAD
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/HEAD
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/config
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/description
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/applypatch-msg.sample
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/commit-msg.sample
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/docs.url
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/fsmonitor-watchman.sample
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/post-update.sample
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/pre-applypatch.sample
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/pre-commit.sample
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/pre-merge-commit.sample
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/pre-push.sample
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/pre-rebase.sample
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/hooks/prepare-commit-msg.sample
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/info/exclude
+-rw-r--r--   0        0        0   100134 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/09/27b8133cfc1ed1c326677f8f1275fae4529606
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/11/666d4d39a077a1996ec6caa4838b6afc4fb766
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/21/fe02781f369270632d786b8f92a2a45877c7d2
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/35/3f973613e5cf238c6f349c80a1ecc73b0721f4
+-rw-r--r--   0        0        0    99164 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/40/12225c0b220d0e1d67001daa7e01bba3df6953
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/49/201e5f0a03c07bc4fdb4a42f3af38849de737d
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/6b/0b1270ff0ca8f03867efcd09ba6ddb6392b1e1
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/6d/6fdfee6f748b293f1edac34acd6827a7e1589e
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/79/7c58e6476d4b262049189b13c012a0c3161a9c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/7f/6df3657f1fd7bc6ac5f382b78106a67cbb8987
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/84/9ddff3b7ec917b5f4563e9a6d3ea63ea512a70
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/85/4c95de2d1dd66585b68262f12d4babdff109d8
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/b5/f6d6162f7f7d8dad33c23d969268c677c70815
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/e9/58a2d705e5dba8ece54cc35122168956fb1c73
+-rw-r--r--   0        0        0    98970 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/f4/a266dd37d5066da46c9a6b8898073ae2930a64
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/ff/0a234106046e297e5c90b8f9a3a110a7c646f5
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/pack/pack-1a28311490079da61bd2022ec284fa8eb1b4bbd1.idx
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/objects/pack/pack-1a28311490079da61bd2022ec284fa8eb1b4bbd1.pack
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/jj/keep/11666d4d39a077a1996ec6caa4838b6afc4fb766
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/jj/keep/49201e5f0a03c07bc4fdb4a42f3af38849de737d
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/jj/keep/904112f02a4e3f7e5100d1332d49f87438439cc0
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/jj/keep/b5f6d6162f7f7d8dad33c23d969268c677c70815
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/jj/keep/e958a2d705e5dba8ece54cc35122168956fb1c73
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/store/git/refs/remotes/github/main
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/repo/submodule_store/type
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/working_copy/checkout
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/working_copy/tree_state
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.jj/working_copy/type
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/src/chadplotlib/__init__.py
+-rw-r--r--   0        0        0   198120 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Bold.ttf
+-rw-r--r--   0        0        0   197756 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Medium.ttf
+-rw-r--r--   0        0        0   197624 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Regular.ttf
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/LICENSE
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 chadplotlib-0.0.2/PKG-INFO
```

### Comparing `chadplotlib-0.0.1/src/chadplotlib/__init__.py` & `chadplotlib-0.0.2/src/chadplotlib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     font_manager.fontManager.addfont(path=path)
     path = importlib.resources.files(__name__).joinpath("fonts/Montserrat-Medium.ttf")
     font_manager.fontManager.addfont(path=path)
     path = importlib.resources.files(__name__).joinpath("fonts/Montserrat-Regular.ttf")
     font_manager.fontManager.addfont(path=path)
     mpl.rcParams['font.family'] = 'Montserrat'
     mpl.rcParams['font.weight'] = 800
-    plt.rcParams['figure.facecolor'] = '#f0f0f0'
-    plt.rcParams['axes.facecolor'] = '#f0f0f0'
+    # plt.rcParams['axes.facecolor'] = '#f0f0f0'
     plt.rcParams.update({'font.size': 13})
     print('chad setup ok')
```

### Comparing `chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Bold.ttf` & `chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Bold.ttf`

 * *Files identical despite different names*

### Comparing `chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Medium.ttf` & `chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Medium.ttf`

 * *Files identical despite different names*

### Comparing `chadplotlib-0.0.1/src/chadplotlib/fonts/Montserrat-Regular.ttf` & `chadplotlib-0.0.2/src/chadplotlib/fonts/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `chadplotlib-0.0.1/LICENSE` & `chadplotlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chadplotlib-0.0.1/pyproject.toml` & `chadplotlib-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chadplotlib"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Théo Daron", email="theo@daron.be" },
   { name="Maxime Deboeck", email="no-mail@plz.be"}
 ]
 description = "Styling options for matplotlib."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `chadplotlib-0.0.1/PKG-INFO` & `chadplotlib-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chadplotlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Styling options for matplotlib.
 Project-URL: Homepage, https://github.com/tdaron/chadplotlib
 Project-URL: Issues, https://github.com/tdaron/chadplotlib/issues
 Author-email: Théo Daron <theo@daron.be>, Maxime Deboeck <no-mail@plz.be>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,17 @@
 `pip install chadplotlib`
 
 ```python
 import chadplotlib
 chadplotlib.makeMeAChad()
 ```
 
+Then just use matplotlib as you would.
+
+
 ## Compiling from scratch 
 Building:
 
 `python3 -m build`
 
 Installing:
```


# Igor Stadnyk
Co-founder & AI Lead of [TrueAI|Trading Co-pilot](https://x.com/truetradingai) and Founding Partner, AI of [INC4](https://x.com/INC_4_), building at the intersection of AI, trading, and Web3 infrastructure.

![AI](https://img.shields.io/badge/AI-4c6ef5)
![Web3](https://img.shields.io/badge/Web3-495057)
![On-chain](https://img.shields.io/badge/On--chain-74b816)

<sub>Robotics · Embedded & field communications · Geospatial systems · AI/data reliability · Web3 infrastructure</sub>

## Open Source

I work on focused reliability fixes across robotics, embedded and field communications, geospatial systems, and AI/data tooling.

### Merged upstream

- [`open-rmf/rmf_ros2#543`](https://github.com/open-rmf/rmf_ros2/pull/543) — fixed the phase key used to publish skip requests.
- [`pylessard/python-can-isotp#160`](https://github.com/pylessard/python-can-isotp/pull/160) — handled reserved STmin values according to ISO 15765-2.
- [`fsspec/filesystem_spec#2102`](https://github.com/fsspec/filesystem_spec/pull/2102) — kept live block-cache instances usable after pickling.

### Current contribution work

- AI/data reliability and compilation: [`joblib/joblib#1840`](https://github.com/joblib/joblib/pull/1840), [`apache/tvm#20141`](https://github.com/apache/tvm/pull/20141)
- HTTP networking reliability: [`urllib3/urllib3#5186`](https://github.com/urllib3/urllib3/pull/5186) — rewinds seekable file-like request bodies before `PoolManager` redirect resends.
- Geospatial I/O: [`geopandas/pyogrio#693`](https://github.com/geopandas/pyogrio/pull/693)
- Robotics, autonomy, and field communications: [`aerostack2/aerostack2#987`](https://github.com/aerostack2/aerostack2/pull/987), [`brian7704/OpenTAKServer#363`](https://github.com/brian7704/OpenTAKServer/pull/363), [`brian7704/OpenTAKServer#364`](https://github.com/brian7704/OpenTAKServer/pull/364), [`PointCloudLibrary/pcl#6464`](https://github.com/PointCloudLibrary/pcl/pull/6464), [`PointCloudLibrary/pcl#6465`](https://github.com/PointCloudLibrary/pcl/pull/6465), [`BehaviorTree/BehaviorTree.CPP#1191`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1191), [`isl-org/Open3D#7536`](https://github.com/isl-org/Open3D/pull/7536)

<sub>These items are open and under upstream review; they are not listed as merged contributions.</sub>

### Upstream review

<sub>GitHub records 40 pull-request review contributions in August 2026.</sub>

- [`libspatialindex#303`](https://github.com/libspatialindex/libspatialindex/pull/303) and [`fmt#4892`](https://github.com/fmtlib/fmt/pull/4892) — requested changes at exact heads `d9905ec` and `ee0b93c`: finite aggregate margins can still overflow into the sentinel-index BUS crash, while the formatter head fails GCC 13 shadow and clang-format 21 gates; both PRs remain open and unmerged.
- [`OctoMap#449`](https://github.com/OctoMap/octomap/pull/449) — approved exact head `1d619b7` after an embedded-build base RED/head GREEN oracle, explicit-Debug and standalone controls, focused unit execution, and 6/6 live checks; the PR remains open and unmerged.
- [`httpcore#1096`](https://github.com/encode/httpcore/pull/1096) — approved exact head `0890100` after reproducing the documented stream-iteration contract mismatch on base/current `master`, then validating 100 exact-head matches plus focused tests, Ruff, mypy, and 7/7 live checks; the PR remains open and unmerged.
- [`lz4#1789`](https://github.com/lz4/lz4/pull/1789) and [`lz4#1777`](https://github.com/lz4/lz4/pull/1777) — approved exact heads `2432c6b` and `f18a372` after ASan reproduced an invalid-block allocation overflow and frame/legacy multi-file suffix overflows on base; both heads reject or safely round-trip the failing inputs under sanitizer and focused test gates, and both PRs remain open and unmerged.
- [`nats.py#1008`](https://github.com/nats-io/nats.py/pull/1008) — approved exact head `dcf8fcd` after a 90-case base/head oracle confirmed the restored NATS timeout-exception contract, with compile hygiene and 27/27 live checks; the PR remains open and unmerged.
- [`fmt#4895`](https://github.com/fmtlib/fmt/pull/4895) — approved exact head `7449a2b` after reproducing incorrect default alignment for nonfinite values on base/current main and passing a seven-case oracle plus 139 format tests; the PR remains open and unmerged.
- [`fsspec#2097`](https://github.com/fsspec/filesystem_spec/pull/2097) and [`lz4#1788`](https://github.com/lz4/lz4/pull/1788) — requested changes at exact heads `4544763` and `a06d8a1`: a missing cache lookup creates a ghost LRU entry that evicts valid values, while late frame-parameter validation mutates an active compression context after returning an error; both PRs remain open and unmerged.
- [`python-lz4#334`](https://github.com/python-lz4/python-lz4/pull/334) — requested changes at exact head `3f85fd8` after proving that both `METH_NOARGS` callbacks retained one-parameter signatures that are undefined behavior under CPython and fail Clang's strict function-type check; the PR remains open and unmerged.
- [`msgspec#1124`](https://github.com/msgspec/msgspec/pull/1124) — approved exact head `58ae07b` after base RED, 50 schema-decoder cases, full unit suites, and current-main integration; the PR remains open and unmerged.
- [`uber-go/zap#1569`](https://github.com/uber-go/zap/pull/1569) — approved exact head `814a458` after reproducing the base panic, repeated focused regression checks, and the full Go suite; the PR remains open and unmerged.
- [`google/go-cmp#402`](https://github.com/google/go-cmp/pull/402) — approved exact head `b455d2a` after base RED, 729 valid-ordering cases repeated 20×, and the full Go suite; the PR remains open and unmerged.
- [`python-lz4#333`](https://github.com/python-lz4/python-lz4/pull/333) — requested changes at exact head `b1979d5` after tracing a failure-path exception-class reference leak in both C extension modules despite 36 green checks; the PR remains open and unmerged.
- [`aiofiles#226`](https://github.com/Tinche/aiofiles/pull/226) — approved exact-head async iteration and context-manager support for `scandir` after base RED, head GREEN, and 222 passing project tests.
- [`BehaviorTree.CPP#1185`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1185) — approved a trace-write clamp after an exact-base ASan oracle reproduced an out-of-bounds read on long event names.
- [`BehaviorTree.CPP#1186`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1186) — approved the integer-width preservation fix after checking its dispatch boundary and regression coverage.
- [`BehaviorTree.CPP#1192`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1192) — reproduced a root-blackboard remap crash and approved the exact-head fix after a local RED/GREEN check.
- [`fsspec#2106`](https://github.com/fsspec/filesystem_spec/pull/2106) — reproduced async deletion beyond `maxdepth` and approved the exact-head boundary fix after the full async target passed.
- [`fsspec#2103`](https://github.com/fsspec/filesystem_spec/pull/2103) — reproduced an archive member escaping the requested local destination and approved the exact-head containment guard after current-master integration tests.
- [`jsonschema#1522`](https://github.com/python-jsonschema/jsonschema/pull/1522) — approved the exact-head fix that distinguishes no patterns from a valid empty regex after base RED, focused, full-suite, and current-main integration checks.
- [`python-lz4#331`](https://github.com/python-lz4/python-lz4/pull/331) — approved the exact-head Cython output-parser fix after base RED, an adversarial parser/concurrency matrix, 5,438 project tests, and 36 green live checks.
- [`redis-py#4288`](https://github.com/redis/redis-py/pull/4288) — approved the exact-head async write guard after base RED, a 10-case close-race and error-translation matrix, current-main integration, and 368 green live checks.
- [`tokio-rs/bytes#839`](https://github.com/tokio-rs/bytes/pull/839) — approved the exact-head signed integer sign-extension fix after base RED, 876 focused cases, full current-main integration, and 18 green live checks; the PR remains open and unmerged.
- [`urllib3#5163`](https://github.com/urllib3/urllib3/pull/5163) — approved exact-head Latin-1 normalization of byte-valued headers after six-path base RED, an exhaustive 256-byte roundtrip, 54 focused tests, current-main integration, and 37 green live checks; the PR remains open and unmerged.
- [`fsspec#2101`](https://github.com/fsspec/filesystem_spec/pull/2101) — proved that the async `filecache` range path still redownloaded the full object because successful downloads never entered the metadata cache.
- [`AnyIO#1294`](https://github.com/agronholm/anyio/pull/1294) — found that the first OS-refused datagram still completed successfully while the new backpressure only blocked the following send.
- [`ImageIO#1203`](https://github.com/imageio/imageio/pull/1203) — caught a broad exception handler that hid invariant and plugin failures from the project's image fuzzer.
- [`Shapely#2465`](https://github.com/shapely/shapely/pull/2465) — found a pickle/deepcopy precision-restoration path that erased pointwise-collapsed line geometry instead of preserving its coordinates.
- [`PyVista#8957`](https://github.com/pyvista/pyvista/pull/8957) — found that malformed negative legacy cell counts could trap the new diagnostic parser in a non-progress loop instead of raising.
- [`pydicom#2337`](https://github.com/pydicom/pydicom/pull/2337) — found that an unknown-VR error translation also mislabeled documented extension-hook failures as malformed DICOM input.
- [`python-can#2089`](https://github.com/hardbyte/python-can/pull/2089) — caught an unrelated workflow change that replaced two immutable Coveralls Action commit pins with a mutable release tag.
- [`pyserial#868`](https://github.com/pyserial/pyserial/pull/868) — found that narrowed RFC 2217 exception handling leaked an allocated socket and reader thread when an interrupt aborted port reconfiguration.
- [`msgspec#1164`](https://github.com/msgspec/msgspec/pull/1164) — found that a metaclass-selection fix bypassed custom construction hooks and their documented struct configuration.
- [`nats.py#1007`](https://github.com/nats-io/nats.py/pull/1007) — found a supported token-only credential form left exposed by a log-redaction patch and requested a focused regression.
- [`OpenTAKServer#362`](https://github.com/brian7704/OpenTAKServer/pull/362) — caught a syntax failure and locale mappings to unavailable catalogs before merge.
- [`pyogrio#691`](https://github.com/geopandas/pyogrio/pull/691), [`cantools#830`](https://github.com/cantools/cantools/pull/830), and [`OpenTAKServer#349`](https://github.com/brian7704/OpenTAKServer/pull/349) — reproduced merge-blocking error-handling and shared-state regressions and submitted concrete `CHANGES_REQUESTED` reviews.

### True Trading (TrueAI)
Building **AI-native trading infrastructure**.
- Native AI agents for on-chain trading
- Focus on execution logic, risk systems, and transparency
- Turning AI from analysis tools into **decision + action systems**

Trading is the entry point.  
The long-term goal is **trustable autonomous systems** for financial markets.

### Web3 & Infrastructure
Building and using foundational infrastructure for AI-driven on-chain systems.
- Reliable infra for AI agents operating on-chain
- Performance, availability, and composability
- Infrastructure designed for **real-time autonomous execution**

## My Vision
- Build products that make complex systems usable  
- Turn intelligence into **real, on-chain outcomes**  
- Help AI and Web3 create real value, not just narratives
   
## Connect With Me
- [Twitter](https://x.com/AIgorStadnyk)
- [LinkedIn](https://www.linkedin.com/in/stadnykigor/)

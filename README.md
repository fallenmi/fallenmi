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
- Geospatial I/O: [`geopandas/pyogrio#693`](https://github.com/geopandas/pyogrio/pull/693)
- Robotics, autonomy, and field communications: [`aerostack2/aerostack2#987`](https://github.com/aerostack2/aerostack2/pull/987), [`brian7704/OpenTAKServer#363`](https://github.com/brian7704/OpenTAKServer/pull/363), [`brian7704/OpenTAKServer#364`](https://github.com/brian7704/OpenTAKServer/pull/364), [`PointCloudLibrary/pcl#6464`](https://github.com/PointCloudLibrary/pcl/pull/6464), [`PointCloudLibrary/pcl#6465`](https://github.com/PointCloudLibrary/pcl/pull/6465), [`BehaviorTree/BehaviorTree.CPP#1191`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1191), [`isl-org/Open3D#7536`](https://github.com/isl-org/Open3D/pull/7536)

<sub>These items are open and under upstream review; they are not listed as merged contributions.</sub>

### Upstream review

- [`BehaviorTree.CPP#1185`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1185) — approved a trace-write clamp after an exact-base ASan oracle reproduced an out-of-bounds read on long event names.
- [`BehaviorTree.CPP#1186`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1186) — approved the integer-width preservation fix after checking its dispatch boundary and regression coverage.
- [`BehaviorTree.CPP#1192`](https://github.com/BehaviorTree/BehaviorTree.CPP/pull/1192) — reproduced a root-blackboard remap crash and approved the exact-head fix after a local RED/GREEN check.
- [`fsspec#2106`](https://github.com/fsspec/filesystem_spec/pull/2106) — reproduced async deletion beyond `maxdepth` and approved the exact-head boundary fix after the full async target passed.
- [`AnyIO#1294`](https://github.com/agronholm/anyio/pull/1294) — found that the first OS-refused datagram still completed successfully while the new backpressure only blocked the following send.
- [`ImageIO#1203`](https://github.com/imageio/imageio/pull/1203) — caught a broad exception handler that hid invariant and plugin failures from the project's image fuzzer.
- [`Shapely#2465`](https://github.com/shapely/shapely/pull/2465) — found a pickle/deepcopy precision-restoration path that erased pointwise-collapsed line geometry instead of preserving its coordinates.
- [`PyVista#8957`](https://github.com/pyvista/pyvista/pull/8957) — found that malformed negative legacy cell counts could trap the new diagnostic parser in a non-progress loop instead of raising.
- [`pydicom#2337`](https://github.com/pydicom/pydicom/pull/2337) — found that an unknown-VR error translation also mislabeled documented extension-hook failures as malformed DICOM input.
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



## 注解powergraph
从优秀的代码中学习

```c
.
├── aggregation
│   ├── aggregation_includes.hpp
│   ├── CMakeLists.txt
│   └── distributed_aggregator.hpp
├── CMakeLists.txt
├── docs
│   ├── faq.dox
│   ├── overview.dox
│   ├── using.dox
│   └── using_warp.dox
├── engine
│   ├── async_consistent_engine.hpp
│   ├── CMakeLists.txt
│   ├── distributed_chandy_misra.hpp
│   ├── engine_includes.hpp
│   ├── execution_status.hpp
│   ├── iengine.hpp
│   ├── message_array.hpp
│   ├── omni_engine.hpp
│   ├── synchronous_engine.hpp
│   ├── warp_engine.hpp
│   ├── warp_graph_broadcast.hpp
│   ├── warp_graph_mapreduce.hpp
│   ├── warp_graph_transform.hpp
│   └── warp_parfor_all_vertices.hpp
├── graph
│   ├── builtin_parsers.hpp
│   ├── CMakeLists.txt
│   ├── distributed_graph.hpp
│   ├── dynamic_local_graph.hpp
│   ├── graph_basic_types.hpp
│   ├── graph_formats.dox
│   ├── graph_gather_apply.hpp
│   ├── graph_hash.hpp
│   ├── graph_includes.hpp
│   ├── graph_ops.hpp
│   ├── graph_storage_deprecated.hpp
│   ├── graph_vertex_join.hpp
│   ├── ingress
│   │   ├── distributed_batch_ingress.hpp
│   │   ├── distributed_constrained_batch_ingress.hpp
│   │   ├── distributed_constrained_oblivious_ingress.hpp
│   │   ├── distributed_constrained_random_ingress.hpp
│   │   ├── distributed_hdrf_ingress.hpp
│   │   ├── distributed_identity_ingress.hpp
│   │   ├── distributed_ingress_base.hpp
│   │   ├── distributed_oblivious_ingress.hpp
│   │   ├── distributed_random_ingress.hpp
│   │   ├── ingress_edge_decision.hpp
│   │   └── sharding_constraint.hpp
│   ├── local_edge_buffer.hpp
│   ├── local_graph.hpp
│   ├── local_graph_ops.hpp
│   └── vertex_set.hpp
├── jni
│   ├── CMakeLists.txt
│   ├── java_any.cpp
│   ├── java_any.hpp
│   ├── org_graphlab_Aggregator.cpp
│   ├── org_graphlab_Aggregator.h
│   ├── org_graphlab_Aggregator.hpp
│   ├── org_graphlab_Context.cpp
│   ├── org_graphlab_Context.h
│   ├── org_graphlab_Context.hpp
│   ├── org_graphlab_Core.cpp
│   ├── org_graphlab_Core.h
│   ├── org_graphlab_Core.hpp
│   ├── org_graphlab_Updater.cpp
│   ├── org_graphlab_Updater.h
│   └── org_graphlab_Updater.hpp
├── logger
│   ├── assertions.hpp
│   ├── assertions.hpp.orig
│   ├── backtrace.cpp
│   ├── backtrace.hpp
│   ├── CMakeLists.txt
│   ├── fail_method.hpp
│   ├── logger.cpp
│   ├── logger.hpp
│   └── logger_includes.hpp
├── macros_def.hpp
├── macros_undef.hpp
├── options
│   ├── CMakeLists.txt
│   ├── command_line_options.cpp
│   ├── command_line_options.hpp
│   ├── engine_help.txt
│   ├── graph_help.txt
│   ├── graphlab_options.hpp
│   ├── options_includes.hpp
│   ├── options_map.cpp
│   └── options_map.hpp
├── parallel
│   ├── atomic_add_vector2_empty_specialization.hpp
│   ├── atomic.hpp
│   ├── atomic_ops.hpp
│   ├── cache_line_pad.hpp
│   ├── CMakeLists.txt
│   ├── deferred_rwlock.hpp
│   ├── fiber_barrier.hpp
│   ├── fiber_conditional.hpp
│   ├── fiber_control.cpp
│   ├── fiber_control.hpp
│   ├── fiber_group.cpp
│   ├── fiber_group.hpp
│   ├── fiber_remote_request.hpp
│   ├── lockfree_push_back.hpp
│   ├── mutex.hpp
│   ├── parallel_includes.hpp
│   ├── pthread_tools.cpp
│   ├── pthread_tools.hpp
│   ├── queued_rwlock.hpp
│   ├── thread_pool.cpp
│   └── thread_pool.hpp
├── rpc
│   ├── async_consensus.cpp
│   ├── async_consensus.hpp
│   ├── buffered_exchange.hpp
│   ├── caching_dht.hpp
│   ├── circular_char_buffer.cpp
│   ├── circular_char_buffer.hpp
│   ├── circular_iovec_buffer.hpp
│   ├── CMakeLists.txt
│   ├── dc_buffered_stream_send2.cpp
│   ├── dc_buffered_stream_send2.hpp
│   ├── dc_comm_base.hpp
│   ├── dc_compile_parameters.hpp
│   ├── dc.cpp
│   ├── dc_dist_object_base.hpp
│   ├── dc_dist_object.hpp
│   ├── dc.hpp
│   ├── dc_init_from_env.cpp
│   ├── dc_init_from_env.hpp
│   ├── dc_init_from_mpi.cpp
│   ├── dc_init_from_mpi.hpp
│   ├── dc_init_from_zookeeper.cpp
│   ├── dc_init_from_zookeeper.hpp
│   ├── dc_internal_types.hpp
│   ├── dc_packet_mask.hpp
│   ├── dc_receive.hpp
│   ├── dc_send.hpp
│   ├── dc_services.hpp
│   ├── dc_stream_receive.cpp
│   ├── dc_stream_receive.hpp
│   ├── dc_tcp_comm.cpp
│   ├── dc_tcp_comm.hpp
│   ├── dc_thread_get_send_buffer.hpp
│   ├── dc_types.hpp
│   ├── delta_dht.cpp
│   ├── delta_dht.hpp
│   ├── dht.hpp
│   ├── distributed_event_log.cpp
│   ├── distributed_event_log.hpp
│   ├── evwrapdef.h
│   ├── evwrapundef.h
│   ├── fiber_async_consensus.cpp
│   ├── fiber_async_consensus.hpp
│   ├── fiber_buffered_exchange.hpp
│   ├── function_arg_types_def.hpp
│   ├── function_arg_types_undef.hpp
│   ├── function_broadcast_issue.hpp
│   ├── function_call_dispatch.hpp
│   ├── function_call_issue.hpp
│   ├── function_ret_type.hpp
│   ├── get_current_process_hash.cpp
│   ├── get_current_process_hash.hpp
│   ├── is_rpc_call.hpp
│   ├── lazy_dht.hpp
│   ├── mem_function_arg_types_def.hpp
│   ├── mem_function_arg_types_undef.hpp
│   ├── object_broadcast_issue.hpp
│   ├── object_call_dispatch.hpp
│   ├── object_call_issue.hpp
│   ├── object_request_dispatch.hpp
│   ├── object_request_issue.hpp
│   ├── pod_template_structs.hpp
│   ├── request_dispatch.hpp
│   ├── request_future.hpp
│   ├── request_issue.hpp
│   ├── request_reply_handler.cpp
│   ├── request_reply_handler.hpp
│   ├── rpc.dox
│   ├── rpc_includes.hpp
│   ├── sample_sort.hpp
│   ├── thread_local_send_buffer.cpp
│   └── thread_local_send_buffer.hpp
├── scheduler
│   ├── CMakeLists.txt
│   ├── fifo_scheduler.cpp
│   ├── fifo_scheduler.hpp
│   ├── get_message_priority.hpp
│   ├── ischeduler.hpp
│   ├── priority_scheduler.cpp
│   ├── priority_scheduler.hpp
│   ├── queued_fifo_scheduler.cpp
│   ├── queued_fifo_scheduler.hpp
│   ├── scheduler_factory.hpp
│   ├── scheduler_includes.hpp
│   ├── scheduler_list.cpp
│   ├── scheduler_list.hpp
│   ├── sweep_scheduler.cpp
│   └── sweep_scheduler.hpp
├── serialization
│   ├── basic_types.hpp
│   ├── CMakeLists.txt
│   ├── conditional_serialize.hpp
│   ├── has_load.hpp
│   ├── has_save.hpp
│   ├── iarchive.hpp
│   ├── is_pod.hpp
│   ├── iterator.hpp
│   ├── list.hpp
│   ├── map.hpp
│   ├── oarchive.hpp
│   ├── serializable_concept.hpp
│   ├── serializable_pod.hpp
│   ├── serialization.dox
│   ├── serialization_includes.hpp
│   ├── serialize.hpp
│   ├── serialize_to_from_string.hpp
│   ├── set.hpp
│   ├── unordered_map.hpp
│   ├── unordered_set.hpp
│   ├── unsupported_serialize.hpp
│   └── vector.hpp
├── ui
│   ├── CMakeLists.txt
│   ├── graphlab_visualization.js
│   ├── index.html
│   ├── intel_demo
│   │   ├── graph_builder.json
│   │   ├── graphlab_visualization.js
│   │   ├── index.html
│   │   └── style.css
│   ├── metrics_server.cpp
│   ├── metrics_server.hpp
│   ├── mongoose
│   │   ├── CMakeLists.txt
│   │   ├── LICENSE
│   │   ├── mongoose.cpp
│   │   └── mongoose.h
│   └── style.css
├── util
│   ├── binary_parser.hpp
│   ├── blocking_queue.hpp
│   ├── bloom_filter.hpp
│   ├── branch_hints.hpp
│   ├── cache.hpp
│   ├── chandy_misra2.hpp
│   ├── chandy_misra.hpp
│   ├── chandy_misra_lockfree.hpp
│   ├── char_counting_sink.hpp
│   ├── charstream.hpp
│   ├── CMakeLists.txt
│   ├── cuckoo_map.hpp
│   ├── cuckoo_map_pow2.hpp
│   ├── cuckoo_set_pow2.hpp
│   ├── dense_bitset.hpp
│   ├── empty.hpp
│   ├── event_log.cpp
│   ├── event_log.hpp
│   ├── fast_multinomial.hpp
│   ├── fiber_blocking_queue.hpp
│   ├── fs_util.cpp
│   ├── fs_util.hpp
│   ├── generate_pds.hpp
│   ├── generics
│   │   ├── any.cpp
│   │   ├── any.hpp
│   │   ├── blob.hpp
│   │   ├── block_linked_list.hpp
│   │   ├── CMakeLists.txt
│   │   ├── conditional_addition_wrapper.hpp
│   │   ├── conditional_combiner_wrapper.hpp
│   │   ├── counting_sort.hpp
│   │   ├── csr_storage.hpp
│   │   ├── dynamic_block.hpp
│   │   ├── dynamic_csr_storage.hpp
│   │   ├── float_selector.hpp
│   │   ├── integer_selector.hpp
│   │   ├── remove_member_pointer.hpp
│   │   ├── robust_cast.hpp
│   │   ├── shuffle.hpp
│   │   ├── test_function_or_functor_type.hpp
│   │   └── vector_zip.hpp
│   ├── hash_functions.hpp
│   ├── hashstream.hpp
│   ├── hdfs.cpp
│   ├── hdfs.hpp
│   ├── hopscotch_map.hpp
│   ├── hopscotch_set.hpp
│   ├── hopscotch_table.hpp
│   ├── inplace_lf_queue2.hpp
│   ├── inplace_lf_queue.cpp
│   ├── inplace_lf_queue.hpp
│   ├── integer_mix.hpp
│   ├── integer_selector.hpp
│   ├── lock_free_internal.hpp
│   ├── lock_free_pool.hpp
│   ├── memory_info.cpp
│   ├── memory_info.hpp
│   ├── mpi_tools.cpp
│   ├── mpi_tools.hpp
│   ├── mutable_queue.hpp
│   ├── net_util.cpp
│   ├── net_util.hpp
│   ├── random.cpp
│   ├── random.hpp
│   ├── resizing_array_sink.hpp
│   ├── safe_circular_char_buffer.cpp
│   ├── safe_circular_char_buffer.hpp
│   ├── small_map.hpp
│   ├── small_set.hpp
│   ├── stl_util.hpp
│   ├── synchronized_unordered_map2.hpp
│   ├── synchronized_unordered_map.hpp
│   ├── system_usage.hpp
│   ├── timer.cpp
│   ├── timer.hpp
│   ├── tracepoint.cpp
│   ├── tracepoint.hpp
│   ├── uint128.hpp
│   ├── union_find.hpp
│   ├── util_includes.hpp
│   ├── web_util.cpp
│   └── web_util.hpp
├── version.hpp
├── vertex_program
│   ├── CMakeLists.txt
│   ├── context.hpp
│   ├── icontext.hpp
│   ├── ivertex_program.hpp
│   ├── messages.hpp
│   ├── op_plus_eq_concept.hpp
│   └── vertex_program_includes.hpp
├── warp.hpp
└── zookeeper
    ├── key_value.cpp
    ├── key_value.hpp
    ├── server_list.cpp
    ├── server_list.hpp
    ├── zookeeper_common.cpp
    └── zookeeper_common.hpp
```
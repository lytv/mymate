# Graph Report - .  (2026-07-27)

## Corpus Check
- Large corpus: 232 files · ~597,715 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 659 nodes · 866 edges · 107 communities (55 shown, 52 thin omitted)
- Extraction: 84% EXTRACTED · 11% INFERRED · 0% AMBIGUOUS · INFERRED: 95 edges (avg confidence: 0.86)
- Token cost: 59,769 input · 14,000 output

## Community Hubs (Navigation)
- Core Script Infrastructure
- Library Function Reference Network
- Agent Supervision & Extension System
- Task Lifecycle & Delivery Pipeline
- Runtime Backend Architecture
- Backend Adapter Implementations
- Backend Abstraction Contract
- Project & Secondmate Management
- PreToolUse Hook Plugins
- Test Patterns & Incidents
- Configuration & Dispatch
- Secondmate Lifecycle
- Fleet Navigation & Backlog
- Pi Extension System
- Safety Gate & Lock System
- CD Guard & Seatbelt Checks
- Architecture Contracts
- Watcher Command Policy
- Liveness & Marker Protocol
- Update & Tangle Guard
- Bootstrap & Skills Registry
- Watch Classifier & State
- Wake Daemon Lifecycle
- Command Policy Enforcement
- Harness & Dispatch Config
- Session Metadata & Metrics
- Wake Queue & Lock Safety
- Captain & Identity Model
- Crew State & Brief System
- Instruction Owner Skills
- Cluster 30
- Cluster 31
- Cluster 32
- Cluster 33
- Cluster 34
- Cluster 35
- Cluster 36
- Cluster 37
- Cluster 38
- Cluster 39
- Cluster 40
- Cluster 41
- Cluster 42
- Cluster 43
- Cluster 44
- Cluster 45
- Cluster 46
- Cluster 47
- Cluster 48
- Cluster 49
- Cluster 50
- Cluster 51
- Cluster 52
- Cluster 53
- Cluster 54
- Cluster 55
- Cluster 56
- Cluster 57
- Cluster 58
- Cluster 59
- Cluster 60
- Cluster 61
- Cluster 62
- Cluster 63
- Cluster 64
- Cluster 65
- Cluster 66
- Cluster 68
- Cluster 69
- Cluster 70
- Cluster 71
- Cluster 72
- Cluster 73
- Cluster 75
- Cluster 76
- Cluster 77
- Cluster 78
- Cluster 79
- Cluster 80
- Cluster 81
- Cluster 82
- Cluster 83
- Cluster 84
- Cluster 85
- Cluster 86
- Cluster 87
- Cluster 88
- Cluster 89
- Cluster 90
- Cluster 91
- Cluster 92
- Cluster 93
- Cluster 94
- Cluster 95
- Cluster 96
- Cluster 97
- Cluster 98
- Cluster 99
- Cluster 100
- Cluster 101
- Cluster 102
- Cluster 103
- Cluster 104
- Cluster 105
- Cluster 106

## God Nodes (most connected - your core abstractions)
1. `herdr.sh - herdr session-provider adapter (EXPERIMENTAL)` - 14 edges
2. `Harness adapters reference skill` - 12 edges
3. `secondmate-provisioning skill` - 12 edges
4. `Away mode (AFK) - captain absence supervision` - 10 edges
5. `cmux.sh - cmux session-provider adapter (EXPERIMENTAL)` - 10 edges
6. `Pi extension background wake supervision` - 10 edges
7. `Claude background-notify supervision` - 9 edges
8. `Grok background-notify supervision` - 9 edges
9. `Secondmate Lifecycle E2E Flow` - 8 edges
10. `X-Mode Relay Connector` - 8 edges

## Surprising Connections (you probably didn't know these)
- `Away mode (AFK) - captain absence supervision` --conceptually_related_to--> `Turn-End Guard Backstop`  [INFERRED]
  bin/fm-afk-launch.sh → AGENTS.md
- `Turn-End Guard Backstop` --conceptually_related_to--> `Watcher supervision cycle`  [INFERRED]
  AGENTS.md → .pi/extensions/fm-primary-pi-watch.ts
- `Harness adapters reference skill` --references--> `Pi primary watcher bridge extension`  [EXTRACTED]
  .agents/skills/harness-adapters/SKILL.md → .pi/extensions/fm-primary-pi-watch.ts
- `Crew dispatch profile rules` --references--> `Harness adapters reference skill`  [EXTRACTED]
  docs/examples/crew-dispatch.json → .agents/skills/harness-adapters/SKILL.md
- `Away-mode supervision skill` --implements--> `Away mode (AFK) - captain absence supervision`  [EXTRACTED]
  .agents/skills/afk/SKILL.md → bin/fm-afk-launch.sh

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Herdr Incident-Driven Fix Progression** — concept_herdr_self_kill_incident_20260702, concept_herdr_respawn_husk_incident_20260703, concept_composer_submit_incident_20260707, concept_workspace_per_home_isolation, concept_herdr_eventwait_push_escalation [INFERRED 0.85]
- **Three-Layer Backend Test Architecture** — concept_backend_fakebin_pattern, concept_backend_parallel_adapter_structure, concept_backend_test_safety_pattern, concept_backend_old_vs_new_conformance [INFERRED 0.95]
- **Test Framework** — tests_lib_sh, tests_secondmate_helpers_sh, tests_wake_helpers_sh [EXTRACTED 1.00]
- **cd-guard Multi-Harness Seatbelt System** — bin_fm_cd_pretool_check_sh, bin_fm_cd_command_policy_mjs, bin_fm_arm_command_policy_mjs, codex_hooks_json, grok_hooks_fm_primary_cd_check_json, opencode_plugins_fm_primary_cd_check_js, pi_extensions_fm_primary_turnend_guard_ts, docs_cd_guard_md [EXTRACTED 1.00]
- **Captain Translation Contract Cross-Reference Network** — agents_md, agents_skills_bootstrap_diagnostics_skill_md, agents_skills_afk_skill_md, agents_skills_decision_hold_lifecycle_skill_md, agents_skills_stuck_crewmate_recovery_skill_md, agents_skills_harness_adapters_skill_md, agents_skills_firstmate_codexapp_skill_md, agents_skills_fmx_respond_skill_md, agents_skills_updatefirstmate_skill_md [EXTRACTED 1.00]
- **Instruction Owner Skills Suite** — agents_skills_diagnostic_reasoning_skill_md, agents_skills_project_management_skill_md, agents_skills_harness_adapters_skill_md, agents_skills_firstmate_coding_guidelines_skill_md, agents_skills_stuck_crewmate_recovery_skill_md, agents_skills_secondmate_provisioning_skill_md, docs_configuration_md, agents_md, bin_fm_brief_sh [EXTRACTED 1.00]
- **Gate Refuse Capability Removal System** — bin_fm_gate_refuse_lib_sh, bin_fm_spawn_sh, bin_fm_send_sh, bin_fm_teardown_sh, no_mistakes_yaml [EXTRACTED 1.00]
- **Lint Parity Guard System** — bin_fm_lint_sh, github_workflows_ci_yml, no_mistakes_yaml, bin_fm_install_shellcheck_sh [EXTRACTED 1.00]
- **Composer Content Safety System** — bin_fm_composer_lib_sh, bin_fm_tmux_lib_sh, bin_fm_peek_sh, rationale_composer_shell_glyph_safety, rationale_ghost_text_robustness [EXTRACTED 1.00]
- **Grok Harness Security System** — bin_fm_spawn_sh, bin_fm_teardown_sh, bin_fm_lock_sh [EXTRACTED 1.00]
- **Backlog Handoff Pipeline** — bin_fm_backlog_handoff_sh, data_backlog_md, data_secondmates_md [EXTRACTED 1.00]
- **Secondmate Lifecycle Pipeline** — tests_fm_secondmate_lifecycle_e2e_flow, tests_fm_secondmate_lifecycle_seed_contracts, tests_fm_secondmate_lifecycle_spawn_contracts, tests_fm_secondmate_lifecycle_teardown_contracts [EXTRACTED 1.00]
- **PR Check Artifact Security System** — tests_fm_pr_check_security_canonical_parsing, tests_fm_pr_check_security_static_poll, tests_fm_pr_check_security_private_atomic_artifacts, tests_fm_pr_check_security_non_executing_migration [EXTRACTED 1.00]
- **Secondmate Harness and Inheritance Model** — tests_fm_secondmate_harness_split, tests_fm_secondmate_harness_inheritance, tests_fm_secondmate_harness_model_effort_pin, tests_fm_shared_captain_inheritance_propagation, tests_fm_shared_captain_drift_quarantine [INFERRED 0.95]
- **Send Protocol Timing System** — tests_fm_send_popup_settle_timing, tests_fm_send_settle_pause, tests_fm_send_strict_resolution, tests_fm_send_secondmate_marker_protocol, tests_fm_send_secondmate_marker_trailing_newlines [INFERRED 0.95]
- **Secondmate Safety Invariants** — tests_fm_secondmate_safety_path_boundary, tests_fm_secondmate_safety_delimiter_refusal, tests_fm_secondmate_safety_active_home_refusal, tests_fm_secondmate_safety_child_worktree_protection, tests_fm_secondmate_safety_no_mistakes_init_new_clones, tests_fm_secondmate_safety_fm_home_parameterization, tests_fm_secondmate_safety_lock_per_home [EXTRACTED 1.00]
- **Dispatch Profile Resolution System** — tests_fm_spawn_dispatch_profile, tests_fm_spawn_dispatch_profile_harness_flags, tests_fm_spawn_batch_dispatch [EXTRACTED 1.00]
- **Session Start Digest System** — tests_fm_session_start_lock_refusal, tests_fm_session_start_context_digest, tests_fm_session_start_endpoint_liveness, tests_fm_session_start_supervision_block, tests_fm_session_start_pi_diagnostics [EXTRACTED 1.00]
- **Test framework foundations** — tests_lib_sh_lib_sh, tests_lib_sh_fm_test_tmproot, tests_lib_sh_fm_test_assertions, tests_lib_sh_fm_git_identity, tests_wake_helpers_sh_wake_helpers, tests_wake_helpers_sh_wake_test_fixtures, tests_secondmate_helpers_sh_secondmate_helpers, tests_secondmate_helpers_sh_fake_tmux_for_secondmate [INFERRED 0.95]
- **Watcher and supervision safety tests** — tests_fm_supervision_events_test_sh_supervision_events_test, tests_fm_supervision_instructions_test_sh_supervision_instructions_test, tests_fm_turnend_guard_test_sh_turnend_guard_test, tests_fm_watch_triage_test_sh_watch_triage_test, tests_fm_watcher_lock_test_sh_watcher_lock_test, tests_fm_watch_checkpoint_test_sh_watch_checkpoint_test [INFERRED 0.95]
- **Wake queue and lifecycle tests** — tests_fm_wake_queue_test_sh_wake_queue_test, tests_fm_wake_daemon_lifecycle_e2e_test_sh_wake_daemon_lifecycle_e2e_test, tests_fm_wake_queue_test_sh_fm_wake_drain_sh, tests_fm_wake_queue_test_sh_fm_wake_lib_sh [INFERRED 0.95]
- **Safety guard tests for destructive operations** — tests_herdr_test_safety_sh_herdr_test_safety, tests_herdr_test_safety_sh_fm_herdr_lab_sh, tests_zellij_test_safety_sh_zellij_test_safety, tests_zellij_test_safety_sh_zellij_test_safety_guard, tests_fm_tangle_guard_test_sh_tangle_guard_test, tests_fm_tangle_guard_test_sh_fm_primary_tangle_branch, tests_fm_teardown_test_sh_teardown_test, tests_fm_teardown_test_sh_landed_work_detection, tests_fm_teardown_test_sh_stale_index_lock_recovery [INFERRED 0.95]
- **Transition record and policy contract tests** — tests_fm_transition_lib_test_sh_transition_lib_test, tests_fm_transition_lib_test_sh_fm_transition_record, tests_fm_transition_lib_test_sh_fm_transition_policy, tests_fm_supervision_events_test_sh_handle_push_transition [INFERRED 0.95]
- **Fleet management and update tests** — tests_fm_update_test_sh_update_test, tests_fm_update_test_sh_fm_update_sh, tests_fm_update_test_sh_instruction_surface_detection, tests_fm_x_mode_test_sh_x_mode_test, tests_fm_x_mode_test_sh_fm_x_poll_sh, tests_fm_x_mode_test_sh_fm_x_reply_sh, tests_fm_x_mode_test_sh_fm_bootstrap_x_activation, tests_fm_x_mode_test_sh_curl_fakebin_for_relay [INFERRED 0.85]
- **Away-mode daemon lifecycle system** — bin_fm-afk-launch_away_mode_daemon_terminal_lifecycle, bin_fm-afk-start_away_mode_daemon_entry, bin_fm-afk-return_return_catch_up_gate, bin_fm-supervise-daemon_sub_supervisor_daemon, concept_away_mode, concept_stale_artifact_lifecycle [EXTRACTED 0.95]
- **Shell command policy system (arm + cd-guard)** — bin_fm-arm-command-policy_arm_command_semantic_policy, bin_fm-arm-pretool-check_arm_pretool_transport, bin_fm-cd-command_policy_cd_guard_policy, bin_fm-cd-pretool-check_cd_guard_transport, concept_command_policy_arm_watcher, concept_command_policy_cd_guard, concept_prefilter_strict_superset [EXTRACTED 0.95]
- **Runtime backend abstraction system** — bin_fm-backend_runtime_backend_abstraction, bin_fm-backend-hometag-lib_home_tag_derivation, concept_backend_abstraction, concept_home_tag_collision_prevention [EXTRACTED 0.95]
- **Primary-to-secondmate config inheritance propagation system** — bin_fm-config-inherit-lib_config_inheritance_propagation, bin_fm-config-push_config_push, concept_config_inheritance, concept_crew_dispatch_selection [EXTRACTED 0.95]
- **Wake classification and crew state system** — bin_fm-classify-lib_wake_classifier, bin_fm-crew-state_crew_current_state_reader, concept_wake_classifier_vocabulary, concept_crew_state_reconciliation [EXTRACTED 0.95]
- **Secondmate fleet management system** — bin_fm-backlog-handoff_backlog_handoff, bin_fm-bootstrap_bootstrap_detection, concept_secondmate_backlog_handoff, concept_secondmate_liveness_sweep, concept_config_inheritance [INFERRED 0.85]
- **Crewmate workflow and brief lifecycle** — bin_fm-brief_crewmate_brief_scaffolder, bin_fm-decision-hold_decision_hold_mechanics, bin_fm-dispatch-select_dispatch_profile_selector, concept_crewmate_brief_scaffold, concept_decision_hold_lifecycle, concept_crew_dispatch_selection [INFERRED 0.85]
- **Fleet snapshot and bearings projection system** — bin_fm-bearings-snapshot_bearings_projection, bin_fm-bootstrap_bootstrap_detection, concept_bearings_snapshot, concept_fleet_snapshot, concept_bootstrap_fleet_sweep [INFERRED 0.85]
- **Custom watcher check hash-verification system** — bin_fm-check-lib_custom_check_verification, bin_fm-check-register_custom_check_registration, concept_custom_check_hash_verification [EXTRACTED 0.95]
- **hyper_pr_merge_pipeline** — bin_fm_pr_check_sh, bin_fm_pr_check_migrate_sh, bin_fm_pr_lib_sh, bin_fm_pr_poll_sh, bin_fm_pr_merge_sh [1.0]
- **hyper_fleet_view_pipeline** — bin_fm_fleet_view_sh, bin_fm_fleet_snapshot_sh [1.0]
- **hyper_ff_machinery** — bin_fm_ff_lib_sh, bin_fm_fleet_sync_sh, bin_fm_merge_local_sh [1.0]
- **hyper_lock_machinery** — bin_fm_lock_lib_sh, bin_fm_lock_sh, bin_fm_guard_sh [1.0]
- **hyper_marker_lib_consumers** — bin_fm_marker_lib_sh, bin_fm_pr_check_sh, bin_fm_pr_merge_sh, bin_fm_pr_poll_sh, bin_fm_merge_local_sh, bin_fm_peek_sh, bin_fm_herdr_lab_sh, bin_fm_fleet_sync_sh, bin_fm_lock_sh, bin_fm_lint_sh, bin_fm_fleet_view_sh, bin_fm_home_seed_sh, bin_fm_guard_sh [1.0]
- **hyper_gate_refuse_consumers** — bin_fm_gate_refuse_lib_sh, bin_fm_herdr_lab_sh, bin_fm_merge_local_sh, bin_fm_pr_merge_sh [1.0]
- **hyper_secondmate_provisioning** — bin_fm_home_seed_sh, bin_fm_fleet_snapshot_sh, bin_fm_fleet_sync_sh, data_secondmates_md, config_secondmate_harness [0.95]
- **hyper_task_state_files** — state_meta_file, bin_fm_fleet_snapshot_sh, bin_fm_pr_check_sh, bin_fm_pr_merge_sh, bin_fm_pr_poll_sh, bin_fm_guard_sh [1.0]
- **Session lifecycle scripts** — bin_fm_session_start_sh_fm_session_start, bin_fm_wake_drain_sh_fm_wake_drain, bin_fm_teardown_sh_fm_teardown, bin_fm_lock_sh_fm_lock, bin_fm_bootstrap_sh_fm_bootstrap, bin_fm_promote_sh_fm_promote [EXTRACTED 1.00]
- **Task management and dispatch scripts** — bin_fm_spawn_sh_fm_spawn, bin_fm_send_sh_fm_send, bin_fm_teardown_sh_fm_teardown, bin_fm_promote_sh_fm_promote, bin_fm_project_mode_sh_fm_project_mode, bin_fm_review_diff_sh_fm_review_diff [EXTRACTED 1.00]
- **Watcher supervision and away-mode system** — bin_fm_supervise_daemon_sh_fm_supervise_daemon, bin_fm_supervision_instructions_sh_fm_supervision_instructions, bin_fm_supervision_lib_sh_fm_supervision_lib, bin_fm_supervisor_target_lib_sh_fm_supervisor_target_lib, bin_fm_turnend_guard_sh_fm_turnend_guard, bin_fm_turnend_guard_grok_sh_fm_turnend_guard_grok, bin_fm_watch_arm_sh_fm_watch_arm, bin_fm_watch_checkpoint_sh_fm_watch_checkpoint, bin_fm_watch_sh_fm_watch, bin_fm_guard_sh_fm_guard [EXTRACTED 1.00]
- **Shared bash libraries sourced by multiple scripts** — bin_fm_wake_lib_sh_fm_wake_lib, bin_fm_tmux_lib_sh_fm_tmux_lib, bin_fm_transition_lib_sh_fm_transition_lib, bin_fm_tangle_lib_sh_fm_tangle_lib, bin_fm_tasks_axi_lib_sh_fm_tasks_axi_lib, bin_fm_composer_lib_sh_fm_composer_lib, bin_fm_classify_lib_sh_fm_classify_lib, bin_fm_backend_sh_fm_backend, bin_fm_gate_refuse_lib_sh_fm_gate_refuse_lib, bin_fm_marker_lib_sh_fm_marker_lib, bin_fm_pr_lib_sh_fm_pr_lib, bin_fm_ff_lib_sh_fm_ff_lib, bin_fm_lock_lib_sh_fm_lock_lib [EXTRACTED 1.00]
- **Guard scripts ensuring supervision integrity** — bin_fm_guard_sh_fm_guard, bin_fm_turnend_guard_sh_fm_turnend_guard, bin_fm_turnend_guard_grok_sh_fm_turnend_guard_grok, bin_fm_gate_refuse_lib_sh_fm_gate_refuse_lib, bin_fm_supervision_lib_sh_fm_supervision_lib [INFERRED 0.95]
- **Git operations scripts** — bin_fm_review_diff_sh_fm_review_diff, bin_fm_update_sh_fm_update, bin_fm_ff_lib_sh_fm_ff_lib, bin_fm_tangle_lib_sh_fm_tangle_lib [INFERRED 0.85]
- **X-Mode Relay Connector System** — firstmate_bin_fm_x_lib_sh, firstmate_bin_fm_x_poll_sh, firstmate_bin_fm_x_reply_sh, firstmate_bin_fm_x_dismiss_sh, firstmate_bin_fm_x_link_sh, firstmate_bin_fm_x_followup_sh, firstmate_concept_x_mode_connector, firstmate_concept_x_mode_mention, firstmate_concept_followup_link_lifecycle, firstmate_concept_reply_context_resolution, firstmate_concept_dry_run_preview [EXTRACTED 1.00]
- **Watcher Supervision & Wake Classification** — firstmate_bin_fm_watch_sh, firstmate_bin_fm_wake_lib_sh, firstmate_bin_fm_classify_lib_sh, firstmate_bin_fm_backend_sh, firstmate_bin_fm_transition_lib_sh, firstmate_bin_fm_check_lib_sh, firstmate_bin_fm_pr_lib_sh, firstmate_bin_fm_x_lib_sh, firstmate_concept_watcher_supervision_loop, firstmate_concept_stale_detection_system, firstmate_concept_heartbeat_fleet_scan [EXTRACTED 1.00]
- **Reply Context Resolution Stack** — firstmate_bin_fmx_context_registry_set, firstmate_bin_fmx_context_registry_get, firstmate_bin_fmx_context_registry_prune, firstmate_bin_fmx_context_registry_clear, firstmate_bin_fmx_request_inbox_context, firstmate_bin_fmx_request_relay_context, firstmate_bin_fmx_resolve_reply_context, firstmate_bin_fmx_extract_reply_context, firstmate_bin_fmx_reply_limit_for_platform, firstmate_concept_reply_context_resolution [EXTRACTED 1.00]
- **Follow-Up Link Lifecycle Stack** — firstmate_bin_fmx_meta_get, firstmate_bin_fmx_meta_link_set, firstmate_bin_fmx_meta_followups_set, firstmate_bin_fmx_meta_link_clear, firstmate_bin_fmx_meta_tmp, firstmate_bin_fm_x_link_sh, firstmate_bin_fm_x_followup_sh, firstmate_concept_followup_link_lifecycle [EXTRACTED 1.00]
- **Runtime session backend ecosystem** — docs_tmux_backend_reference, docs_herdr_backend_experimental, docs_zellij_backend_experimental, docs_cmux_backend_experimental, docs_orca_backend_experimental, docs_codexapp_backend_blocked, docs_architecture_runtime_backend_abstract_class, docs_configuration_runtime_backend_selection [EXTRACTED 1.00]
- **Primary-session PreToolUse guard family** — docs_armpretoolcheck_watcher_seatbelt, docs_cdguard_cd_seatbelt, docs_turnendguard_no_turn_ends_blind, docs_architecture_pre_tool_use_seatbelt_family, docs_armpretoolcheck_command_policy_mjs, docs_cdguard_command_policy_mjs, docs_turnendguard_shared_predicate [EXTRACTED 1.00]
- **Herdr slash command send incident chain** — docs_herdr_backend_slash_command_send_incident, docs_herdr_backend_composer_state_structural_read, docs_herdr_backend_experimental [EXTRACTED 1.00]
- **Captain decision hold lifecycle system** — docs_decisionholdlifecycle_captain_decision_hold, docs_decisionholdlifecycle_fm_decision_hold_sh, docs_decisionholdlifecycle_decision_key_identity, docs_decisionholdlifecycle_scout_teardown_gate, docs_decisionholdlifecycle_blocked_by_resolution [EXTRACTED 1.00]
- **Away-mode wedge alarm system** — docs_wedgealarm_active_alert, docs_wedgealarm_alert_channels, docs_wedgealarm_test_safety_seam, docs_wedgealarm_rate_limiting, docs_wedgealarm_incident_20260710, docs_architecture_away_mode_supervisor [EXTRACTED 1.00]
- **X mode public mention relay system** — docs_architecture_x_mode, docs_configuration_x_mode_config, docs_configuration_reply_splitting [EXTRACTED 1.00]
- **Knowledge routing and memory policy** — docs_architecture_memory_routing_policy, docs_architecture_inspect_then_update, docs_architecture_stow_knowledge_routing [EXTRACTED 1.00]
- **Session Lifecycle Management Pattern** — sessions_session_lifecycle, sessions_session_restoration, sessions_duration_tracking, sessions_session_metrics [INFERRED 0.75]
- **All five session-provider backend adapters implementing the common interface** — bin_backends_tmux_sh, bin_backends_herdr_sh, bin_backends_zellij_sh, bin_backends_cmux_sh, bin_backends_orca_sh [EXTRACTED 1.00]
- **Backends sharing fm-composer-lib.sh for composer state classification** — bin_backends_cmux_sh, bin_backends_herdr_sh, bin_backends_orca_sh, bin_fm_composer_lib_sh [EXTRACTED 1.00]
- **Backends using fm-backend-hometag-lib.sh for cross-home collision prevention** — bin_backends_cmux_sh, bin_backends_zellij_sh, bin_fm_backend_hometag_lib_sh [EXTRACTED 1.00]
- **Herdr push-escalation pipeline: herdr.sh orchestrates herdr-eventwait.py through fm-transition-lib.sh** — bin_backends_herdr_sh, bin_backends_herdr_eventwait_py, bin_fm_transition_lib_sh [EXTRACTED 1.00]
- **Firstmate Identity System** — concept_firstmate, concept_captain, concept_crewmate, concept_secondmate [EXTRACTED 1.00]
- **Configuration System** — config_backend, config_crew_harness, config_crew_dispatch, config_secondmate_harness, config_backlog_backend [EXTRACTED 1.00]
- **Task Lifecycle** — concept_ship_task, concept_scout_task, concept_delivery_mode, concept_brief, concept_backlog [EXTRACTED 1.00]
- **Supervision Stack** — concept_event_watcher, concept_wake_queue, concept_session_lock, concept_turnend_guard, concept_away_mode [EXTRACTED 1.00]
- **Repository File Layout** — agents_md, claude_md, contributing_md, readme_md, skills_lock_json, no_mistakes_yaml [EXTRACTED 1.00]
- **Common supervision prerequisites (drain, x-mode, away-mode check)** — docs_wake_drain, docs_x_mode_sourcing, docs_away_mode [EXTRACTED 1.00]
- **Shell & safety enforcement across harnesses** — docs_pretooluse_seatbelt, docs_shell_ampersand_prohibition, docs_watcher_arm [EXTRACTED 1.00]
- **Harness-specific wake adapter implementations** — docs_background_task_wake, docs_foreground_checkpoint_wake, docs_tui_plugin_wake, docs_extension_wake [EXTRACTED 1.00]
- **PreToolUse guard pair (cd-check + pretool-check)** — opencode_plugins_fm_primary_cd_check, opencode_plugins_fm_primary_pretool_check, plugins_pretooluse_seatbelt, plugins_tool_execute_before_hook [EXTRACTED 1.00]
- **Turn-end and watch arm coordination** — opencode_plugins_fm_primary_turnend_guard, opencode_plugins_fm_primary_watch_arm, plugins_turnend_guard, plugins_watch_arm, plugins_session_idle_event [EXTRACTED 1.00]
- **OpenCode firstmate plugin set** — opencode_plugins_fm_primary_cd_check, opencode_plugins_fm_primary_pretool_check, opencode_plugins_fm_primary_turnend_guard, opencode_plugins_fm_primary_watch_arm, opencode_plugins_package_json [EXTRACTED 1.00]
- **PreToolUse and Stop hook system across harnesses** — grok_hooks_fm_primary_cd_check, grok_hooks_fm_primary_pretool_check, grok_hooks_fm_primary_turnend_guard, claude_settings_json, codex_hooks_json, pi_extensions_fm_primary_turnend_guard, concept_pretool_check, concept_cd_check, concept_turnend_guard [EXTRACTED 1.00]
- **Watcher and away-mode wake delivery system** — pi_extensions_fm_primary_pi_watch, agents_skills_afk_skill_afk, agents_skills_fmx_respond_skill_fmx_respond, concept_watcher_supervision, concept_away_mode, concept_x_mode [EXTRACTED 1.00]
- **CI enforcement pipeline (lint, test, invariant, no-mistakes gate)** — github_workflows_ci, github_workflows_no_mistakes_required, concept_no_mistakes_pipeline [EXTRACTED 1.00]
- **Agent skills cross-referencing network** — agents_skills_afk_skill_afk, agents_skills_bearings_skill_bearings, agents_skills_bootstrap_diagnostics_skill_bootstrap_diagnostics, agents_skills_decision_hold_lifecycle_skill_decision_hold_lifecycle, agents_skills_diagnostic_reasoning_skill_diagnostic_reasoning, agents_skills_firstmate_codexapp_skill_firstmate_codexapp, agents_skills_firstmate_coding_guidelines_skill_firstmate_coding_guidelines, agents_skills_firstmate_orca_skill_firstmate_orca, agents_skills_fmx_respond_skill_fmx_respond, agents_skills_harness_adapters_skill_harness_adapters, agents_skills_axi_skill_axi [INFERRED 0.75]
- **secondmate lifecycle management (create → seed → launch → recover → handoff → retire)** — agents_skills_secondmate_provisioning, secondmate_provisioning_charter, secondmate_provisioning_home_seed, secondmate_provisioning_backlog_handoff, secondmate_provisioning_teardown [EXTRACTED 0.95]
- **knowledge capture and persistence (stow internal + public)** — agents_skills_stow, skills_stow, stow_knowledge_routing, stow_public_tiered_routing, stow_inspect_then_update [EXTRACTED 0.95]
- **fleet maintenance operations (update + recovery + knowledge stow)** — agents_skills_updatefirstmate, agents_skills_stuck_crewmate_recovery, agents_skills_stow [INFERRED 0.75]
- **project lifecycle management (add → create → clone → initialize → remove)** — agents_skills_project_management, project_management_delivery_modes, project_management_registry, project_management_yolo_posture [EXTRACTED 0.95]

## Communities (107 total, 52 thin omitted)

### Community 0 - "Core Script Infrastructure"
Cohesion: 0.10
Nodes (33): fmx_auth_header_file, fmx_context_registry_clear, fmx_context_registry_get, fmx_context_registry_prune, fmx_context_registry_set, fmx_env_get, fmx_extract_reply_context, fmx_image_payload_file (+25 more)

### Community 1 - "Library Function Reference Network"
Cohesion: 0.08
Nodes (35): fm-backend.sh - Backend adapter resolution and validation, fm-bootstrap.sh - Bootstrap diagnostics and mutating sweeps, fm-classify-lib.sh - Shared wake classifier for captain-relevant events, fm-composer-lib.sh - Shared composer-content classification and ghost stripping, fm-ff-lib.sh - Fast-forward library for git operations, fm-gate-refuse-lib.sh - Gate agent mutation refusal, fm-guard.sh - Pull-based supervision guard warning, fm-harness.sh - Primary harness resolution (+27 more)

### Community 2 - "Agent Supervision & Extension System"
Cohesion: 0.14
Nodes (30): Away mode check, Background task completion wake mechanism, Isolated PI_CODING_AGENT_DIR, Extension background wake mechanism, Foreground checkpoint wake mechanism, Generic supervision contract (AGENTS.md), Harness-specific supervision adapter pattern, OpenCode fm-primary-watch-arm plugin (+22 more)

### Community 3 - "Task Lifecycle & Delivery Pipeline"
Cohesion: 0.09
Nodes (19): Backlog Contract, Captain-Private Data, Delivery Mode, Fleet Sync, Knowledge Routing Rules, No-Mistakes Pipeline, Project Management, Scout Task (Knowledge Report) (+11 more)

### Community 4 - "Runtime Backend Architecture"
Cohesion: 0.10
Nodes (10): Backend Adapter Interface, Runtime Backend Auto-Detection, Old-vs-New Backend Refactoring Conformance, Parallel Backend Adapter Structure, Backend Test Safety Guard Pattern, Cmux Unique Safety Concerns, Herdr Native Event Subscription Escalation, 2026-07-03 Herdr Respawn Husk Incident (+2 more)

### Community 5 - "Backend Adapter Implementations"
Cohesion: 0.25
Nodes (18): cmux.sh - cmux session-provider adapter (EXPERIMENTAL), herdr-eventwait.py - AF_UNIX event subscriber for herdr push escalation, herdr.sh - herdr session-provider adapter (EXPERIMENTAL), orca.sh - Orca terminal session-provider adapter, tmux.sh - tmux session-provider adapter (reference backend), zellij.sh - zellij session-provider adapter (EXPERIMENTAL), fm-backend-hometag-lib.sh - shared home-scoped tag derivation for tab/workspace titles, fm-composer-lib.sh - shared composer content classifier and ghost-text stripper (+10 more)

### Community 6 - "Backend Abstraction Contract"
Cohesion: 0.12
Nodes (19): Runtime backend abstract contract (create/send/peek/capture/close/agent_alive), Runtime session backend abstraction, cmux runtime backend (experimental, Ghostty-based macOS terminal), cmux last-in-window teardown (adds sibling default workspace), cmux socket control modes matrix (automation mode recommended), cmux workspace ids do not survive relaunch, Codex App backend (blocked, no supported shell-callable bridge), Codex Desktop host-tool smoke verification (+11 more)

### Community 7 - "Project & Secondmate Management"
Cohesion: 0.17
Nodes (18): project-management skill, secondmate-provisioning skill, stuck-crewmate-recovery skill, updatefirstmate skill, delivery modes (no-mistakes, direct-PR, local-only), project registry (data/projects.md), yolo autonomy posture, backlog handoff (fm-backlog-handoff.sh) (+10 more)

### Community 8 - "PreToolUse Hook Plugins"
Cohesion: 0.19
Nodes (12): fm-arm-pretool-check.sh, arm lifecycle state machine, fm-cd-pretool-check.sh, PreToolUse seatbelt, resolveRoot helper, runProcess helper, session.idle event, tool.execute.before hook (+4 more)

### Community 9 - "Test Patterns & Incidents"
Cohesion: 0.16
Nodes (4): agreements_md, Fakebin Command-Log Testing Pattern, 2026-07-14 Two-Owner Incident, Quota-Balanced Dispatch

### Community 10 - "Configuration & Dispatch"
Cohesion: 0.17
Nodes (15): fm-backend-hometag-lib.sh - shared per-installation home-tag derivation, fm-backend.sh - runtime-backend selection and dispatch abstraction, fm-bearings-snapshot.sh - compact bearings snapshot projector, fm-bootstrap.sh - bootstrap detection, fleet refresh, and installs, fm-config-inherit-lib.sh - inheritance propagation to secondmate homes, fm-config-push.sh - push inherited local material to live secondmate homes, fm-dispatch-select.sh - resolve dispatch rule to concrete profile, Runtime backend abstraction (tmux, herdr, zellij, orca, cmux) (+7 more)

### Community 11 - "Secondmate Lifecycle"
Cohesion: 0.14
Nodes (15): Fast-Forward Library, Spawn Script, Backlog Handoff Script, Home Seed Script, Secondmate Lifecycle E2E Flow, Secondmate Seed Contracts, Secondmate Spawn Contracts, Secondmate Teardown Contracts (+7 more)

### Community 12 - "Fleet Navigation & Backlog"
Cohesion: 0.25
Nodes (4): data/backlog.md, data/secondmates.md, Backlog Handoff Contract, Decision Hold Lifecycle

### Community 13 - "Pi Extension System"
Cohesion: 0.14
Nodes (14): AGENTS.md Document, Pi Primary Watch Extension, Firstmate Respond Restriction, Validate Contract, Worker Owns Synchronous Driver, Pi Primary Live E2E Regression, Pi Watcher Extension Fire, External Healthy Watcher Detection (+6 more)

### Community 14 - "Safety Gate & Lock System"
Cohesion: 0.23
Nodes (3): Gate Refuse Capability Removal, GOTMPDIR Integration, Grok Hook Security

### Community 15 - "CD Guard & Seatbelt Checks"
Cohesion: 0.27
Nodes (11): Firstmate coding guidelines skill, Harness adapters reference skill, Claude settings with PreToolUse and Stop hooks, .codex/hooks.json, CD (checkout) guard check, PreToolUse seatbelt checks, Turn-End Guard Backstop, Grok primary CD check hook (+3 more)

### Community 16 - "Architecture Contracts"
Cohesion: 0.17
Nodes (12): No-mistakes gate authority boundary, Secondmate architecture (isolated persistent firstmate home), Worktree isolation (linked git worktrees for tasks), cd-guard scoped to plain firstmate checkouts only (linked worktree inert), Backlog backend selection (dot-tasks-toml slash config-slash-backlog-backend), FM_HOME operational layout (data slash state slash config slash projects), Blocked-by dependency resolution for held decisions, Decision hold lifecycle for unresolved captain decisions (+4 more)

### Community 17 - "Watcher Command Policy"
Cohesion: 0.20
Nodes (11): Turn-end gap incident (2026-07-04, parked no-mistakes gate unwatched 9 hours), PreToolUse seatbelt family (primary-session guards), fm-arm-command-policy.mjs (semantic owner of watcher-arm classification), Fast-path prefilter (strict superset before classifier delegation), Quoting-decoder marker set (ANSI-C dollar-single-quote and dollar-double-quote), Watcher-arm PreToolUse seatbelt, cd-guard PreToolUse seatbelt (persistent cwd change prevention), fm-cd-command-policy.mjs (semantic owner of cd-guard classification) (+3 more)

### Community 18 - "Liveness & Marker Protocol"
Cohesion: 0.20
Nodes (10): Bootstrap Script, Backend Script, Marker Library, Liveness Convergence, Agent Alive Probe, Secondmate Liveness Sweep, Herdr Secondmate Marker E2E, From-Firstmate Marker Protocol (+2 more)

### Community 19 - "Update & Tangle Guard"
Cohesion: 0.24
Nodes (5): fm-supervision-instructions.sh, fm_primary_tangle_branch, fm-update.sh, instruction surface detection, fake tmux for secondmate tests

### Community 20 - "Bootstrap & Skills Registry"
Cohesion: 0.22
Nodes (6): bootstrap-diagnostics/SKILL.md, firstmate-codexapp/SKILL.md, fmx-respond/SKILL.md, harness-adapters/SKILL.md, updatefirstmate/SKILL.md, Captain Translation Contract

### Community 21 - "Watch Classifier & State"
Cohesion: 0.28
Nodes (9): fm-check-lib.sh - custom watcher-check hash verification library, fm-check-register.sh - bind custom watcher check to current bytes, fm-classify-lib.sh - shared wake classifier and status vocabulary, fm-composer-lib.sh - fleet-wide composer-content classification, fm-crew-state.sh - deterministic crew current-state reader, Composer content classification safety rule, Crew state reconciliation via run-step and pane, Custom watcher-check hash verification (+1 more)

### Community 22 - "Wake Daemon Lifecycle"
Cohesion: 0.28
Nodes (5): watcher+daemon lifecycle, fm-watch-checkpoint.sh, fm-classify-lib.sh, wake triage classifier, wake/daemon test fixtures

### Community 23 - "Command Policy Enforcement"
Cohesion: 0.25
Nodes (4): .grok/hooks/fm-primary-cd-check.json, .opencode/plugins/fm-primary-cd-check.js, .pi/extensions/fm-primary-turnend-guard.ts, cd-guard Design

### Community 24 - "Harness & Dispatch Config"
Cohesion: 0.29
Nodes (7): bin_fm_harness_sh, bin_fm_home_seed_sh, Crewmate Brief Scaffold, Crewmate (Worker Agent), Secondmate (Domain Supervisor), config_crew_harness, config_secondmate_harness

### Community 25 - "Session Metadata & Metrics"
Cohesion: 0.32
Nodes (8): Session with Active Edits (11 edits), Session Duration Tracking, Long-Running Session (~5.9 days), Session Lifecycle (start/restore/end), Claude-Flow Session Metadata, Session Metrics (edits/commands/tasks/errors), Session Restoration, Timestamp-Based Session ID

### Community 26 - "Wake Queue & Lock Safety"
Cohesion: 0.29
Nodes (6): fm-wake-drain.sh, fm-wake-lib.sh, wake-queue safety matrix, fm_pid_identity, fm-watch-arm.sh, watcher lock/singleton safety

### Community 27 - "Captain & Identity Model"
Cohesion: 0.38
Nodes (6): CLAUDE.md Symlink, Captain (Human User), Escalation and Captain Etiquette, Firstmate Orchestrator, Self-Update Mechanism, Yolo Autonomy Flag

### Community 29 - "Instruction Owner Skills"
Cohesion: 0.29
Nodes (5): diagnostic-reasoning/SKILL.md, firstmate-coding-guidelines/SKILL.md, project-management/SKILL.md, secondmate-provisioning/SKILL.md, stuck-crewmate-recovery/SKILL.md

### Community 30 - "Cluster 30"
Cohesion: 0.33
Nodes (7): X mode mention response skill, Event-Driven Bash Watcher, Supervision Protocol, Durable Wake Queue, Watcher supervision cycle, X Mode (Social Integration), Pi primary watcher bridge extension

### Community 31 - "Cluster 31"
Cohesion: 0.38
Nodes (7): stow skill (internal), stow skill (public installer-facing), inspect-then-update curation pattern, knowledge routing via AGENTS.md section 6, .stow-notes.md private fallback file, tiered local-first routing (explicit > local convention > .stow-notes.md fallback), no-skill-storage scope exclusion

### Community 32 - "Cluster 32"
Cohesion: 0.38
Nodes (7): fm-afk-launch.sh - away-mode daemon terminal lifecycle manager, fm-afk-return.sh - deterministic away-mode return catch-up gate, fm-afk-start.sh - away-mode daemon common entry point, fm-supervise-daemon.sh - away-mode sub-supervisor daemon, fm-wake-lib.sh - wake queue and lock library, Away mode (AFK) - captain absence supervision, Away-mode stale artifact lifecycle

### Community 33 - "Cluster 33"
Cohesion: 0.48
Nodes (7): fm-arm-command-policy.mjs - semantic policy for watcher-arm shell commands, fm-arm-pretool-check.sh - stable PreToolUse transport for arm command policy, fm-cd-command-policy.mjs - semantic policy for cd-guard shell commands, fm-cd-pretool-check.sh - stable PreToolUse transport for cd-guard policy, Watcher-arm command policy - protected shell command classification, CD guard policy - prevent persistent directory change in primary checkout, Strict-superset prefilter for command policies

### Community 34 - "Cluster 34"
Cohesion: 0.29
Nodes (5): bin_fm_ff_lib_sh, bin_fm_merge_local_sh, data/captain.md, data/projects.md, Fleet Sync Drift Handling

### Community 35 - "Cluster 35"
Cohesion: 0.48
Nodes (6): bin_fm_marker_lib_sh, bin_fm_pr_check_migrate_sh, bin_fm_pr_check_sh, bin_fm_pr_merge_sh, bin_fm_pr_poll_sh, state_meta_file

### Community 36 - "Cluster 36"
Cohesion: 0.33
Nodes (6): Away-mode supervision skill, Bearings fleet status report skill, Decision hold lifecycle skill, Diagnostic reasoning procedure skill, Firstmate Orca backend operator skill, Crewmate/secondmate lifecycle

### Community 38 - "Cluster 38"
Cohesion: 0.33
Nodes (6): Agent eXperience Interface skill, Bootstrap diagnostics handling skill, Crew dispatch profile routing, Harness adapter system, Firstmate hook/extension system, Crew dispatch profile rules

### Community 39 - "Cluster 39"
Cohesion: 0.33
Nodes (6): fm-backlog-handoff.sh - hand backlog items from main to secondmate, fm-brief.sh - scaffold crewmate brief or secondmate charter, fm-decision-hold.sh - deterministic mechanics for durable captain decisions, Crewmate brief scaffold contract, Durable captain decision hold lifecycle, Secondmate backlog handoff protocol

### Community 40 - "Cluster 40"
Cohesion: 0.33
Nodes (6): Away-mode sub-supervisor (fm-supervise-daemon.sh), Away-mode wedge alarm (active alert channels), Wedge alarm channels (osascript, herdr, command, auto, off), Wedge alarm incident (2026-07-10 claude-on-herdr wedged 8.5 hours), Wedge alarm rate-limiting (at most once per max-defer window), Wedge alarm test safety seam (FM_WEDGE_ALARM_EXEC)

### Community 41 - "Cluster 41"
Cohesion: 0.33
Nodes (4): event_wait_or_sleep, handle_push_transition, fm_transition_policy, fm_transition_record

### Community 42 - "Cluster 42"
Cohesion: 0.50
Nodes (4): fm-pr-check.sh, fm-teardown.sh, landed-work detection, stale index.lock recovery

### Community 43 - "Cluster 43"
Cohesion: 0.40
Nodes (4): fm_supervision_unhealthy, fm-turnend-guard hook, Grok primary hook config, Pi primary turn-end guard extension

### Community 44 - "Cluster 44"
Cohesion: 0.50
Nodes (4): curl fakebin for relay, bootstrap X-mode activation, fm-x-poll.sh, fm-x-reply.sh

### Community 46 - "Cluster 46"
Cohesion: 0.50
Nodes (4): Config Inheritance Library, Shared Captain Drift Quarantine, Shared Captain Preference Propagation, Shared Captain Read-Only Enforcement

### Community 47 - "Cluster 47"
Cohesion: 0.50
Nodes (4): Dispatch Select Script, Batch Dispatch, Dispatch Profile Selection, Harness-Specific Profile Flags

### Community 49 - "Cluster 49"
Cohesion: 0.50
Nodes (4): Dispatch Profile Routing, Runtime Backend Selection, config/backend Runtime Override, config/crew-dispatch.json Profiles

### Community 50 - "Cluster 50"
Cohesion: 0.50
Nodes (4): Durable wake queue (state/.wake-queue), Event-driven supervision, Zero-token bash watcher (fm-watch.sh), Autonomous wake mechanism A (background task re-invocation)

### Community 51 - "Cluster 51"
Cohesion: 0.50
Nodes (4): Session Start Context Digest, Endpoint Liveness Lines, Session Start Lock Refusal Path, Supervision Block Output

### Community 55 - "Cluster 55"
Cohesion: 0.67
Nodes (3): Session Bootstrap Checks, FM_HOME Instance Directory, Session Lock Mechanism

### Community 56 - "Cluster 56"
Cohesion: 0.67
Nodes (3): Inspect-then-update memory writes, Memory routing policy (most-specific owner), /stow knowledge routing and unfinished work sweep

### Community 57 - "Cluster 57"
Cohesion: 0.67
Nodes (3): X mode (public mention relay), X mode reply splitting (platform-aware chunking), X mode configuration (FMX_PAIRING_TOKEN in dot-env)

### Community 58 - "Cluster 58"
Cohesion: 0.67
Nodes (3): Harness support (claude, codex, opencode, pi, grok), Toolchain requirements, Harness-specific turn-end integrations (Stop hook / session.idle)

### Community 59 - "Cluster 59"
Cohesion: 0.67
Nodes (3): The bin slash toolbelt (fm-star lifecycle scripts), fm-decision-hold.sh (decision lifecycle), fm-fleet-snapshot.sh (structured fleet snapshot JSON)

## Ambiguous Edges - Review These
- `orca.sh - Orca terminal session-provider adapter` → `fm-backend-hometag-lib.sh - shared home-scoped tag derivation for tab/workspace titles`  [AMBIGUOUS]
  bin/backends/orca.sh · relation: references

## Knowledge Gaps
- **200 isolated node(s):** `Lexer`, `splitProgram`, `commandPosition`, `cmux_refuse_if_unsafe`, `cmux_safe_close_workspace` (+195 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **52 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `orca.sh - Orca terminal session-provider adapter` and `fm-backend-hometag-lib.sh - shared home-scoped tag derivation for tab/workspace titles`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **Why does `Away mode (AFK) - captain absence supervision` connect `Cluster 32` to `Cluster 36`, `Watch Classifier & State`, `Cluster 30`, `CD Guard & Seatbelt Checks`?**
  _High betweenness centrality (0.037) - this node is a cross-community bridge._
- **Why does `Supervision Protocol` connect `Cluster 30` to `Cluster 32`, `Captain & Identity Model`, `CD Guard & Seatbelt Checks`?**
  _High betweenness centrality (0.030) - this node is a cross-community bridge._
- **Why does `Crewmate/secondmate lifecycle` connect `Cluster 36` to `Task Lifecycle & Delivery Pipeline`, `Project & Secondmate Management`, `CD Guard & Seatbelt Checks`?**
  _High betweenness centrality (0.028) - this node is a cross-community bridge._
- **Are the 4 inferred relationships involving `herdr.sh - herdr session-provider adapter (EXPERIMENTAL)` (e.g. with `cmux.sh - cmux session-provider adapter (EXPERIMENTAL)` and `tmux.sh - tmux session-provider adapter (reference backend)`) actually correct?**
  _`herdr.sh - herdr session-provider adapter (EXPERIMENTAL)` has 4 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Lexer`, `splitProgram`, `commandPosition` to the rest of the system?**
  _230 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Core Script Infrastructure` be split into smaller, more focused modules?**
  _Cohesion score 0.09528214616096208 - nodes in this community are weakly interconnected._
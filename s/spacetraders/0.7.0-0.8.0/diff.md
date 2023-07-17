# Comparing `tmp/spacetraders-0.7.0.tar.gz` & `tmp/spacetraders-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.7.0.tar", max compression
+gzip compressed data, was "spacetraders-0.8.0.tar", max compression
```

## Comparing `spacetraders-0.7.0.tar` & `spacetraders-0.8.0.tar`

### file list

```diff
@@ -1,232 +1,236 @@
--rw-r--r--   0        0        0     3472 2023-06-24 20:27:51.914738 spacetraders-0.7.0/README.md
--rw-r--r--   0        0        0      664 2023-06-24 20:46:22.094297 spacetraders-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-06-24 20:29:35.619679 spacetraders-0.7.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-06-24 20:29:32.919850 spacetraders-0.7.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:32.999539 spacetraders-0.7.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     4125 2023-06-24 20:29:37.266883 spacetraders-0.7.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:33.000673 spacetraders-0.7.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4693 2023-06-24 20:29:37.260816 spacetraders-0.7.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5626 2023-06-24 20:29:37.256620 spacetraders-0.7.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4597 2023-06-24 20:29:37.258777 spacetraders-0.7.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4420 2023-06-24 20:29:37.264954 spacetraders-0.7.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     4971 2023-06-24 20:29:37.262957 spacetraders-0.7.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:32.933836 spacetraders-0.7.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     4349 2023-06-24 20:29:37.254483 spacetraders-0.7.0/spacetraders/api/default/get_status.py
--rw-r--r--   0        0        0     7032 2023-06-24 20:29:37.252421 spacetraders-0.7.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:32.997177 spacetraders-0.7.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4405 2023-06-24 20:29:37.260808 spacetraders-0.7.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4976 2023-06-24 20:29:37.258693 spacetraders-0.7.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:33.006677 spacetraders-0.7.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     5084 2023-06-24 20:29:37.252290 spacetraders-0.7.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4934 2023-06-24 20:29:37.269622 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     5041 2023-06-24 20:29:37.274022 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     5265 2023-06-24 20:29:37.252336 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     6196 2023-06-24 20:29:37.274124 spacetraders-0.7.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     5279 2023-06-24 20:29:37.275010 spacetraders-0.7.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5757 2023-06-24 20:29:37.258716 spacetraders-0.7.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4482 2023-06-24 20:29:37.273105 spacetraders-0.7.0/spacetraders/api/fleet/get_mounts.py
--rw-r--r--   0        0        0     4425 2023-06-24 20:29:37.263003 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4499 2023-06-24 20:29:37.267434 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4988 2023-06-24 20:29:37.269241 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     5562 2023-06-24 20:29:37.270076 spacetraders-0.7.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4414 2023-06-24 20:29:37.271452 spacetraders-0.7.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     5734 2023-06-24 20:29:37.266779 spacetraders-0.7.0/spacetraders/api/fleet/install_mount.py
--rw-r--r--   0        0        0     4905 2023-06-24 20:29:37.271231 spacetraders-0.7.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5999 2023-06-24 20:29:37.267846 spacetraders-0.7.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     5985 2023-06-24 20:29:37.256613 spacetraders-0.7.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     5533 2023-06-24 20:29:37.269555 spacetraders-0.7.0/spacetraders/api/fleet/negotiate_contract.py
--rw-r--r--   0        0        0     5382 2023-06-24 20:29:37.254358 spacetraders-0.7.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5209 2023-06-24 20:29:37.272140 spacetraders-0.7.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     6004 2023-06-24 20:29:37.273035 spacetraders-0.7.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     5550 2023-06-24 20:29:37.271640 spacetraders-0.7.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     5599 2023-06-24 20:29:37.272066 spacetraders-0.7.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5558 2023-06-24 20:29:37.265577 spacetraders-0.7.0/spacetraders/api/fleet/remove_mount.py
--rw-r--r--   0        0        0     5318 2023-06-24 20:29:37.256437 spacetraders-0.7.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5679 2023-06-24 20:29:37.261097 spacetraders-0.7.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5929 2023-06-24 20:29:37.268935 spacetraders-0.7.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     5633 2023-06-24 20:29:37.254472 spacetraders-0.7.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-06-24 20:29:32.986313 spacetraders-0.7.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     5135 2023-06-24 20:29:37.260834 spacetraders-0.7.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5369 2023-06-24 20:29:37.254413 spacetraders-0.7.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     5091 2023-06-24 20:29:37.265086 spacetraders-0.7.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4469 2023-06-24 20:29:37.252252 spacetraders-0.7.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5554 2023-06-24 20:29:37.263180 spacetraders-0.7.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4930 2023-06-24 20:29:37.258779 spacetraders-0.7.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4914 2023-06-24 20:29:37.256673 spacetraders-0.7.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4384 2023-06-24 20:29:36.106117 spacetraders-0.7.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-06-24 20:29:36.024133 spacetraders-0.7.0/spacetraders/errors.py
--rw-r--r--   0        0        0    15600 2023-06-24 20:29:36.227660 spacetraders-0.7.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-24 20:29:37.273588 spacetraders-0.7.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1332 2023-06-24 20:29:37.275575 spacetraders-0.7.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1662 2023-06-24 20:29:37.267518 spacetraders-0.7.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1666 2023-06-24 20:29:37.271683 spacetraders-0.7.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1898 2023-06-24 20:29:37.274449 spacetraders-0.7.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     2260 2023-06-24 20:29:37.269929 spacetraders-0.7.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1712 2023-06-24 20:29:37.274921 spacetraders-0.7.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1340 2023-06-24 20:29:37.274496 spacetraders-0.7.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1685 2023-06-24 20:29:37.273114 spacetraders-0.7.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-06-24 20:29:33.411910 spacetraders-0.7.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1744 2023-06-24 20:29:37.273296 spacetraders-0.7.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1251 2023-06-24 20:29:37.274448 spacetraders-0.7.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1469 2023-06-24 20:29:37.257059 spacetraders-0.7.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.251912 spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1448 2023-06-24 20:29:37.253238 spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1316 2023-06-24 20:29:37.259029 spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1468 2023-06-24 20:29:37.260487 spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-06-24 20:29:37.269579 spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1488 2023-06-24 20:29:37.268046 spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.275222 spacetraders-0.7.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1430 2023-06-24 20:29:37.259354 spacetraders-0.7.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1470 2023-06-24 20:29:37.260394 spacetraders-0.7.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1275 2023-06-24 20:29:37.257743 spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1356 2023-06-24 20:29:37.255066 spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1292 2023-06-24 20:29:37.251913 spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1227 2023-06-24 20:29:37.257677 spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1368 2023-06-24 20:29:37.255383 spacetraders-0.7.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1281 2023-06-24 20:29:37.270863 spacetraders-0.7.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1572 2023-06-24 20:29:37.267932 spacetraders-0.7.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1369 2023-06-24 20:29:37.259979 spacetraders-0.7.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1370 2023-06-24 20:29:37.263352 spacetraders-0.7.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1866 2023-06-24 20:29:37.270834 spacetraders-0.7.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0      547 2023-06-24 20:29:33.363711 spacetraders-0.7.0/spacetraders/models/faction_symbols.py
--rw-r--r--   0        0        0     1421 2023-06-24 20:29:37.260205 spacetraders-0.7.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     1869 2023-06-24 20:29:33.464077 spacetraders-0.7.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1275 2023-06-24 20:29:37.259694 spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1334 2023-06-24 20:29:37.255161 spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1193 2023-06-24 20:29:37.257297 spacetraders-0.7.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1311 2023-06-24 20:29:37.261772 spacetraders-0.7.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1186 2023-06-24 20:29:37.251912 spacetraders-0.7.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.270313 spacetraders-0.7.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.262583 spacetraders-0.7.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1163 2023-06-24 20:29:37.262053 spacetraders-0.7.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1208 2023-06-24 20:29:37.263245 spacetraders-0.7.0/spacetraders/models/get_mounts_get_mounts_200_response.py
--rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.256954 spacetraders-0.7.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1206 2023-06-24 20:29:37.270565 spacetraders-0.7.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1169 2023-06-24 20:29:37.262033 spacetraders-0.7.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1291 2023-06-24 20:29:37.256300 spacetraders-0.7.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1262 2023-06-24 20:29:37.260599 spacetraders-0.7.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1210 2023-06-24 20:29:37.269398 spacetraders-0.7.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1175 2023-06-24 20:29:37.254866 spacetraders-0.7.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     2628 2023-06-24 20:29:37.271035 spacetraders-0.7.0/spacetraders/models/get_status_response_200.py
--rw-r--r--   0        0        0     1213 2023-06-24 20:29:37.260541 spacetraders-0.7.0/spacetraders/models/get_status_response_200_announcements_item.py
--rw-r--r--   0        0        0     1897 2023-06-24 20:29:37.253760 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards.py
--rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.272512 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
--rw-r--r--   0        0        0     1346 2023-06-24 20:29:37.255422 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
--rw-r--r--   0        0        0     1191 2023-06-24 20:29:37.261039 spacetraders-0.7.0/spacetraders/models/get_status_response_200_links_item.py
--rw-r--r--   0        0        0     1314 2023-06-24 20:29:37.256461 spacetraders-0.7.0/spacetraders/models/get_status_response_200_server_resets.py
--rw-r--r--   0        0        0     1483 2023-06-24 20:29:37.268384 spacetraders-0.7.0/spacetraders/models/get_status_response_200_stats.py
--rw-r--r--   0        0        0     1163 2023-06-24 20:29:37.255075 spacetraders-0.7.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1323 2023-06-24 20:29:37.275267 spacetraders-0.7.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1299 2023-06-24 20:29:37.273759 spacetraders-0.7.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1266 2023-06-24 20:29:37.262895 spacetraders-0.7.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1340 2023-06-24 20:29:37.259253 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response.py
--rw-r--r--   0        0        0     1855 2023-06-24 20:29:37.253675 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response_data.py
--rw-r--r--   0        0        0     1148 2023-06-24 20:29:37.264648 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_request.py
--rw-r--r--   0        0        0     1300 2023-06-24 20:29:37.262150 spacetraders-0.7.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1232 2023-06-24 20:29:37.273013 spacetraders-0.7.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1205 2023-06-24 20:29:37.266835 spacetraders-0.7.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1606 2023-06-24 20:29:37.273250 spacetraders-0.7.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1168 2023-06-24 20:29:37.259392 spacetraders-0.7.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-06-24 20:29:37.271942 spacetraders-0.7.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1409 2023-06-24 20:29:37.265907 spacetraders-0.7.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2398 2023-06-24 20:29:37.263607 spacetraders-0.7.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1880 2023-06-24 20:29:37.274291 spacetraders-0.7.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-06-24 20:29:33.570681 spacetraders-0.7.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2148 2023-06-24 20:29:37.276130 spacetraders-0.7.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-06-24 20:29:33.538978 spacetraders-0.7.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1536 2023-06-24 20:29:37.251920 spacetraders-0.7.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.256356 spacetraders-0.7.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.267932 spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1444 2023-06-24 20:29:37.264238 spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1400 2023-06-24 20:29:37.252033 spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
--rw-r--r--   0        0        0     1259 2023-06-24 20:29:37.261520 spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.264151 spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1231 2023-06-24 20:29:37.267085 spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1420 2023-06-24 20:29:37.271428 spacetraders-0.7.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1214 2023-06-24 20:29:37.261379 spacetraders-0.7.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1352 2023-06-24 20:29:37.254578 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1558 2023-06-24 20:29:37.262169 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1322 2023-06-24 20:29:37.268620 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1346 2023-06-24 20:29:37.263538 spacetraders-0.7.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.265131 spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1511 2023-06-24 20:29:37.265279 spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1546 2023-06-24 20:29:37.263768 spacetraders-0.7.0/spacetraders/models/refuel_ship_json_body.py
--rw-r--r--   0        0        0     1245 2023-06-24 20:29:37.252030 spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1616 2023-06-24 20:29:37.258230 spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1628 2023-06-24 20:29:37.260857 spacetraders-0.7.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0     1232 2023-06-24 20:29:37.269174 spacetraders-0.7.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1665 2023-06-24 20:29:37.272872 spacetraders-0.7.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-06-24 20:29:37.274184 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response.py
--rw-r--r--   0        0        0     1851 2023-06-24 20:29:37.264571 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py
--rw-r--r--   0        0        0     1179 2023-06-24 20:29:37.263145 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_request.py
--rw-r--r--   0        0        0     2482 2023-06-24 20:29:37.258559 spacetraders-0.7.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1170 2023-06-24 20:29:37.264382 spacetraders-0.7.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1166 2023-06-24 20:29:37.267376 spacetraders-0.7.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1174 2023-06-24 20:29:37.258826 spacetraders-0.7.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1174 2023-06-24 20:29:37.254277 spacetraders-0.7.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1709 2023-06-24 20:29:37.253710 spacetraders-0.7.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2451 2023-06-24 20:29:37.260669 spacetraders-0.7.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.255599 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1542 2023-06-24 20:29:37.266731 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1323 2023-06-24 20:29:37.259214 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3230 2023-06-24 20:29:37.254032 spacetraders-0.7.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1504 2023-06-24 20:29:37.266323 spacetraders-0.7.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1510 2023-06-24 20:29:37.258883 spacetraders-0.7.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2248 2023-06-24 20:29:37.269821 spacetraders-0.7.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-06-24 20:29:33.313610 spacetraders-0.7.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     2135 2023-06-24 20:29:37.263267 spacetraders-0.7.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-06-24 20:29:33.254096 spacetraders-0.7.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2904 2023-06-24 20:29:37.274828 spacetraders-0.7.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-06-24 20:29:33.478392 spacetraders-0.7.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1709 2023-06-24 20:29:37.264749 spacetraders-0.7.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1451 2023-06-24 20:29:37.258181 spacetraders-0.7.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1812 2023-06-24 20:29:37.258141 spacetraders-0.7.0/spacetraders/models/ship_modification_transaction.py
--rw-r--r--   0        0        0     2306 2023-06-24 20:29:37.268133 spacetraders-0.7.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-06-24 20:29:33.277679 spacetraders-0.7.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     2226 2023-06-24 20:29:37.264182 spacetraders-0.7.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-06-24 20:29:33.515951 spacetraders-0.7.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-06-24 20:29:33.333297 spacetraders-0.7.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     2114 2023-06-24 20:29:37.256214 spacetraders-0.7.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-06-24 20:29:33.336106 spacetraders-0.7.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1891 2023-06-24 20:29:37.262313 spacetraders-0.7.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1650 2023-06-24 20:29:37.274434 spacetraders-0.7.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-06-24 20:29:33.330456 spacetraders-0.7.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     2200 2023-06-24 20:29:37.266800 spacetraders-0.7.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-06-24 20:29:33.525865 spacetraders-0.7.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1303 2023-06-24 20:29:37.271757 spacetraders-0.7.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-06-24 20:29:33.497285 spacetraders-0.7.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1316 2023-06-24 20:29:37.272261 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response.py
--rw-r--r--   0        0        0     2197 2023-06-24 20:29:37.265176 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py
--rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.252074 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py
--rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.258347 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py
--rw-r--r--   0        0        0     1477 2023-06-24 20:29:37.270018 spacetraders-0.7.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1541 2023-06-24 20:29:37.252123 spacetraders-0.7.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-06-24 20:29:33.265907 spacetraders-0.7.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-06-24 20:29:33.259345 spacetraders-0.7.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     2009 2023-06-24 20:29:37.266832 spacetraders-0.7.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2511 2023-06-24 20:29:37.266673 spacetraders-0.7.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1238 2023-06-24 20:29:37.270611 spacetraders-0.7.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1761 2023-06-24 20:29:37.255242 spacetraders-0.7.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2228 2023-06-24 20:29:37.253937 spacetraders-0.7.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1209 2023-06-24 20:29:37.253331 spacetraders-0.7.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-06-24 20:29:33.611132 spacetraders-0.7.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1918 2023-06-24 20:29:37.265530 spacetraders-0.7.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1213 2023-06-24 20:29:37.266034 spacetraders-0.7.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-06-24 20:29:33.506563 spacetraders-0.7.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1460 2023-06-24 20:29:37.268481 spacetraders-0.7.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1424 2023-06-24 20:29:37.272042 spacetraders-0.7.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-06-24 20:29:33.280231 spacetraders-0.7.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1352 2023-06-24 20:29:37.269510 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1241 2023-06-24 20:29:37.274468 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1453 2023-06-24 20:29:37.269452 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1168 2023-06-24 20:29:37.265632 spacetraders-0.7.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-06-24 20:29:37.265279 spacetraders-0.7.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1436 2023-06-24 20:29:37.261914 spacetraders-0.7.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2510 2023-06-24 20:29:37.257639 spacetraders-0.7.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.253158 spacetraders-0.7.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1215 2023-06-24 20:29:37.256725 spacetraders-0.7.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1427 2023-06-24 20:29:37.275639 spacetraders-0.7.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-06-24 20:29:33.305812 spacetraders-0.7.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-06-24 20:29:33.378026 spacetraders-0.7.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1341 2023-06-24 20:29:37.262762 spacetraders-0.7.0/spacetraders/types.py
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.8.0/README.md
+-rw-r--r--   0        0        0      664 2023-07-17 04:00:19.627740 spacetraders-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-07-17 03:57:36.867745 spacetraders-0.8.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-17 03:57:36.317745 spacetraders-0.8.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.367745 spacetraders-0.8.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     4434 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/agents/get_agent.py
+-rw-r--r--   0        0        0     4882 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/agents/get_agents.py
+-rw-r--r--   0        0        0     4125 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.367745 spacetraders-0.8.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4693 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5626 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4597 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4420 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     4971 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.327745 spacetraders-0.8.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     4349 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/default/get_status.py
+-rw-r--r--   0        0        0     7032 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.367745 spacetraders-0.8.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4405 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4976 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.367745 spacetraders-0.8.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5084 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4934 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     5041 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     5265 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6196 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5279 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5757 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4482 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/get_mounts.py
+-rw-r--r--   0        0        0     4425 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4499 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4988 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     5562 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4414 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     5734 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/install_mount.py
+-rw-r--r--   0        0        0     4905 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5999 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     5985 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5533 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/negotiate_contract.py
+-rw-r--r--   0        0        0     5382 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5209 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     6004 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     5550 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     5599 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5558 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/remove_mount.py
+-rw-r--r--   0        0        0     5318 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5679 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5929 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     5633 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:57:36.357745 spacetraders-0.8.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     5135 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5369 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     5091 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4469 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5554 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4930 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4914 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4384 2023-07-17 03:57:37.177745 spacetraders-0.8.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-07-17 03:57:37.157745 spacetraders-0.8.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    15769 2023-07-17 03:57:37.307745 spacetraders-0.8.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1269 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1332 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1895 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1666 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1898 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     2260 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1712 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1340 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1685 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-07-17 03:57:36.497745 spacetraders-0.8.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1744 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1251 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1469 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1304 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1448 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1316 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1468 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1488 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1257 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1430 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1470 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1275 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1356 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1292 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1227 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1368 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1281 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1572 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1369 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1370 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1866 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0      547 2023-07-17 03:57:36.487745 spacetraders-0.8.0/spacetraders/models/faction_symbols.py
+-rw-r--r--   0        0        0     1421 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     1869 2023-07-17 03:57:36.587745 spacetraders-0.8.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1275 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1334 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1172 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_agent_response_200.py
+-rw-r--r--   0        0        0     1293 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_agents_response_200.py
+-rw-r--r--   0        0        0     1193 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1311 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1186 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1305 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1176 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1163 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1208 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_mounts_get_mounts_200_response.py
+-rw-r--r--   0        0        0     1176 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1206 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1169 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1291 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1262 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1210 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1175 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     2628 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_status_response_200.py
+-rw-r--r--   0        0        0     1213 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_announcements_item.py
+-rw-r--r--   0        0        0     1897 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards.py
+-rw-r--r--   0        0        0     1304 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
+-rw-r--r--   0        0        0     1346 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
+-rw-r--r--   0        0        0     1191 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_links_item.py
+-rw-r--r--   0        0        0     1314 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_server_resets.py
+-rw-r--r--   0        0        0     1483 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_status_response_200_stats.py
+-rw-r--r--   0        0        0     1163 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1323 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1299 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1266 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1340 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_201_response.py
+-rw-r--r--   0        0        0     1855 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_201_response_data.py
+-rw-r--r--   0        0        0     1148 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_request.py
+-rw-r--r--   0        0        0     1300 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1232 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1205 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1606 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1168 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1409 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2398 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1880 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-07-17 03:57:36.507745 spacetraders-0.8.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2148 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-07-17 03:57:36.507745 spacetraders-0.8.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1536 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1176 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1444 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1400 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
+-rw-r--r--   0        0        0     1259 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1231 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1420 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1214 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1352 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1558 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1322 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1346 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1511 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1546 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/refuel_ship_json_body.py
+-rw-r--r--   0        0        0     1245 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1616 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1628 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0     1232 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1665 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_201_response.py
+-rw-r--r--   0        0        0     1851 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py
+-rw-r--r--   0        0        0     1179 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_request.py
+-rw-r--r--   0        0        0     2482 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1170 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1166 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1174 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1174 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1709 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2451 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1304 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1542 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1323 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3230 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1504 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1510 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2248 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-07-17 03:57:36.467745 spacetraders-0.8.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     2135 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-07-17 03:57:36.577745 spacetraders-0.8.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2904 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-07-17 03:57:36.487745 spacetraders-0.8.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1709 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1451 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1812 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_modification_transaction.py
+-rw-r--r--   0        0        0     2306 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-07-17 03:57:36.517745 spacetraders-0.8.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     2226 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-07-17 03:57:36.577745 spacetraders-0.8.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-07-17 03:57:36.577745 spacetraders-0.8.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2114 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-07-17 03:57:36.487745 spacetraders-0.8.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1891 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1650 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-07-17 03:57:36.517745 spacetraders-0.8.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     2200 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-07-17 03:57:36.497745 spacetraders-0.8.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1303 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-07-17 03:57:36.567745 spacetraders-0.8.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1316 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response.py
+-rw-r--r--   0        0        0     2197 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py
+-rw-r--r--   0        0        0     1305 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1305 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py
+-rw-r--r--   0        0        0     1477 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1541 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-07-17 03:57:36.557745 spacetraders-0.8.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-07-17 03:57:36.477745 spacetraders-0.8.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     2009 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2511 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1238 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1761 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2228 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1209 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-07-17 03:57:36.497745 spacetraders-0.8.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1918 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1213 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-07-17 03:57:36.497745 spacetraders-0.8.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1460 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1424 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-07-17 03:57:36.567745 spacetraders-0.8.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1352 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1241 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1453 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1168 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1436 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2510 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1257 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1215 2023-07-17 03:57:37.647745 spacetraders-0.8.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1427 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-07-17 03:57:36.587745 spacetraders-0.8.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-07-17 03:57:36.497745 spacetraders-0.8.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1341 2023-07-17 03:57:37.637745 spacetraders-0.8.0/spacetraders/types.py
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.8.0/PKG-INFO
```

### Comparing `spacetraders-0.7.0/README.md` & `spacetraders-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/pyproject.toml` & `spacetraders-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.7.0"
+version = "0.8.0"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.7.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.8.0/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.8.0/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.8.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.8.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.8.0/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.8.0/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/default/get_status.py` & `spacetraders-0.8.0/spacetraders/api/default/get_status.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/default/register.py` & `spacetraders-0.8.0/spacetraders/api/default/register.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.8.0/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.8.0/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.8.0/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.8.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.8.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.8.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.8.0/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.8.0/spacetraders/api/fleet/extract_resources.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_mounts.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_mounts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.8.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/install_mount.py` & `spacetraders-0.8.0/spacetraders/api/fleet/install_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.8.0/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/jump_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/negotiate_contract.py` & `spacetraders-0.8.0/spacetraders/api/fleet/negotiate_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.8.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.8.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/purchase_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/remove_mount.py` & `spacetraders-0.8.0/spacetraders/api/fleet/remove_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.8.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.8.0/spacetraders/api/fleet/ship_refine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.8.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.8.0/spacetraders/api/fleet/warp_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_system.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_systems.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_systems.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.8.0/spacetraders/api/systems/get_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/client.py` & `spacetraders-0.8.0/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/__init__.py` & `spacetraders-0.8.0/spacetraders/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 from .extraction_yield import ExtractionYield
 from .faction import Faction
 from .faction_symbols import FactionSymbols
 from .faction_trait import FactionTrait
 from .faction_trait_symbol import FactionTraitSymbol
 from .fulfill_contract_response_200 import FulfillContractResponse200
 from .fulfill_contract_response_200_data import FulfillContractResponse200Data
+from .get_agent_response_200 import GetAgentResponse200
+from .get_agents_response_200 import GetAgentsResponse200
 from .get_contract_response_200 import GetContractResponse200
 from .get_contracts_response_200 import GetContractsResponse200
 from .get_faction_response_200 import GetFactionResponse200
 from .get_factions_response_200 import GetFactionsResponse200
 from .get_jump_gate_response_200 import GetJumpGateResponse200
 from .get_market_response_200 import GetMarketResponse200
 from .get_mounts_get_mounts_200_response import GetMountsGetMounts200Response
@@ -241,14 +243,16 @@
     "ExtractResourcesResponse201Data",
     "Faction",
     "FactionSymbols",
     "FactionTrait",
     "FactionTraitSymbol",
     "FulfillContractResponse200",
     "FulfillContractResponse200Data",
+    "GetAgentResponse200",
+    "GetAgentsResponse200",
     "GetContractResponse200",
     "GetContractsResponse200",
     "GetFactionResponse200",
     "GetFactionsResponse200",
     "GetJumpGateResponse200",
     "GetMarketResponse200",
     "GetMountsGetMounts200Response",
```

### Comparing `spacetraders-0.7.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.8.0/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/agent.py` & `spacetraders-0.8.0/spacetraders/models/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
+    Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..types import Unset
+from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Agent")
 
 
 class Agent(BaseModel):
     """Agent details.
 
     Attributes:
-        account_id (str): Account ID that is tied to this agent.
         symbol (str): Symbol of the agent.
         headquarters (str): The headquarters of the agent.
         credits_ (int): The number of credits the agent has available. Credits can be negative if funds have been
             overdrawn.
         starting_faction (str): The faction the agent started with.
+        account_id (Union[Unset, str]): Account ID that is tied to this agent. Only included on your own agent.
+        ship_count (Union[Unset, int]): How many ships are owned by the agent.
     """
 
-    account_id: str = Field(alias="accountId")
     symbol: str = Field(alias="symbol")
     headquarters: str = Field(alias="headquarters")
     credits_: int = Field(alias="credits")
     starting_faction: str = Field(alias="startingFaction")
+    account_id: Union[Unset, str] = Field(UNSET, alias="accountId")
+    ship_count: Union[Unset, int] = Field(UNSET, alias="shipCount")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.7.0/spacetraders/models/chart.py` & `spacetraders-0.8.0/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/connected_system.py` & `spacetraders-0.8.0/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/contract.py` & `spacetraders-0.8.0/spacetraders/models/contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.8.0/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/contract_payment.py` & `spacetraders-0.8.0/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/contract_terms.py` & `spacetraders-0.8.0/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/cooldown.py` & `spacetraders-0.8.0/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.8.0/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.8.0/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.8.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.8.0/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.8.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.8.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.8.0/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.8.0/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/extraction.py` & `spacetraders-0.8.0/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.8.0/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/faction.py` & `spacetraders-0.8.0/spacetraders/models/faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/faction_symbols.py` & `spacetraders-0.8.0/spacetraders/models/faction_symbols.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/faction_trait.py` & `spacetraders-0.8.0/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.8.0/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.8.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_mounts_get_mounts_200_response.py` & `spacetraders-0.8.0/spacetraders/models/get_mounts_get_mounts_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_announcements_item.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_announcements_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_links_item.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_links_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_server_resets.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_server_resets.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_status_response_200_stats.py` & `spacetraders-0.8.0/spacetraders/models/get_status_response_200_stats.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.8.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response.py` & `spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response_data.py` & `spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_request.py` & `spacetraders-0.8.0/spacetraders/models/install_mount_install_mount_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.8.0/spacetraders/models/jettison_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.8.0/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jump_gate.py` & `spacetraders-0.8.0/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.8.0/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.8.0/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/market.py` & `spacetraders-0.8.0/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.8.0/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/market_transaction.py` & `spacetraders-0.8.0/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/meta.py` & `spacetraders-0.8.0/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.8.0/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.8.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py` & `spacetraders-0.8.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py` & `spacetraders-0.8.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.8.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.8.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.8.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.8.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.8.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.8.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.8.0/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/refuel_ship_json_body.py` & `spacetraders-0.8.0/spacetraders/models/refuel_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.8.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/register_json_body.py` & `spacetraders-0.8.0/spacetraders/models/register_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/register_response_201.py` & `spacetraders-0.8.0/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.8.0/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response.py` & `spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py` & `spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_request.py` & `spacetraders-0.8.0/spacetraders/models/remove_mount_remove_mount_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.8.0/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.8.0/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.8.0/spacetraders/models/scanned_ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.8.0/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.8.0/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_system.py` & `spacetraders-0.8.0/spacetraders/models/scanned_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.8.0/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.8.0/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship.py` & `spacetraders-0.8.0/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.8.0/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.8.0/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_crew.py` & `spacetraders-0.8.0/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_engine.py` & `spacetraders-0.8.0/spacetraders/models/ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_frame.py` & `spacetraders-0.8.0/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.8.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.8.0/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.8.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_modification_transaction.py` & `spacetraders-0.8.0/spacetraders/models/ship_modification_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_module.py` & `spacetraders-0.8.0/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.8.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_mount.py` & `spacetraders-0.8.0/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.8.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.8.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_nav.py` & `spacetraders-0.8.0/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.8.0/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.8.0/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.8.0/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.8.0/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response.py` & `spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py` & `spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py` & `spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py` & `spacetraders-0.8.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_registration.py` & `spacetraders-0.8.0/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.8.0/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/ship_type.py` & `spacetraders-0.8.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/shipyard.py` & `spacetraders-0.8.0/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/shipyard_ship.py` & `spacetraders-0.8.0/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.8.0/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.8.0/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/survey.py` & `spacetraders-0.8.0/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.8.0/spacetraders/models/survey_deposit.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/system.py` & `spacetraders-0.8.0/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/system_faction.py` & `spacetraders-0.8.0/spacetraders/models/system_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.8.0/spacetraders/models/system_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/trade_good.py` & `spacetraders-0.8.0/spacetraders/models/trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.8.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.8.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.8.0/spacetraders/models/warp_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.8.0/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.8.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/waypoint.py` & `spacetraders-0.8.0/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.8.0/spacetraders/models/waypoint_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.8.0/spacetraders/models/waypoint_orbital.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/waypoint_trait.py` & `spacetraders-0.8.0/spacetraders/models/waypoint_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.8.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/spacetraders/types.py` & `spacetraders-0.8.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.7.0/PKG-INFO` & `spacetraders-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


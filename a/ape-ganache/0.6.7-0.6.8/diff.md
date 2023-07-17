# Comparing `tmp/ape-ganache-0.6.7.tar.gz` & `tmp/ape-ganache-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ganache-0.6.7.tar", last modified: Tue Jun 13 16:57:39 2023, max compression
+gzip compressed data, was "ape-ganache-0.6.8.tar", last modified: Mon Jul 17 17:08:45 2023, max compression
```

## Comparing `ape-ganache-0.6.7.tar` & `ape-ganache-0.6.8.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.145533 ape-ganache-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.145533 ape-ganache-0.6.7/ape_ganache/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/ape_ganache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/ape_ganache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/ape_ganache/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/ape_ganache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:57:38.000000 ape-ganache-0.6.7/ape_ganache/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.145533 ape-ganache-0.6.7/ape_ganache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 16:57:39.000000 ape-ganache-0.6.7/ape_ganache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.145533 ape-ganache-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.145533 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.141533 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:57:39.153533 ape-ganache-0.6.7/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-13 16:56:37.000000 ape-ganache-0.6.7/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.800978 ape-ganache-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.780978 ape-ganache-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-17 17:08:45.800978 ape-ganache-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.780978 ape-ganache-0.6.8/ape_ganache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/ape_ganache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/ape_ganache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/ape_ganache/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/ape_ganache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.780978 ape-ganache-0.6.8/ape_ganache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 17:08:45.000000 ape-ganache-0.6.8/ape_ganache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 17:08:45.800978 ape-ganache-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.784978 ape-ganache-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.784978 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.776978 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.796978 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.796978 ape-ganache-0.6.8/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:45.800978 ape-ganache-0.6.8/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-07-17 17:07:16.000000 ape-ganache-0.6.8/tests/test_trace.py
```

### Comparing `ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/bug.md` & `ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/feature.md` & `ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ganache-0.6.8/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/release-drafter.yml` & `ape-ganache-0.6.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/codeql.yml` & `ape-ganache-0.6.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/commit.yaml` & `ape-ganache-0.6.8/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/prtitle.yaml` & `ape-ganache-0.6.8/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/publish.yaml` & `ape-ganache-0.6.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/stale-prs.yml` & `ape-ganache-0.6.8/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.github/workflows/test.yaml` & `ape-ganache-0.6.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.gitignore` & `ape-ganache-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/.pre-commit-config.yaml` & `ape-ganache-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/CONTRIBUTING.md` & `ape-ganache-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/LICENSE` & `ape-ganache-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/PKG-INFO` & `ape-ganache-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ganache
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-ganache: Ape network provider for Ganache
 Home-page: https://github.com/ApeWorX/ape-ganache
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ganache-0.6.7/README.md` & `ape-ganache-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/ape_ganache/__init__.py` & `ape-ganache-0.6.8/ape_ganache/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/ape_ganache/exceptions.py` & `ape-ganache-0.6.8/ape_ganache/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/ape_ganache/provider.py` & `ape-ganache-0.6.8/ape_ganache/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,22 +344,31 @@
         receipt = self.chain_manager.get_receipt(txn_hash)
 
         # Subtract base gas costs.
         # (21_000 + 4 gas per 0-byte and 16 gas per non-zero byte).
         data_gas = sum([4 if x == 0 else 16 for x in receipt.data])
         method_gas_cost = receipt.gas_used - 21_000 - data_gas
 
+        if receipt.contract_address:
+            # Deploy txn
+            address = receipt.contract_address
+            call_type = CallType.CREATE
+        else:
+            # Invoke txn
+            address = receipt.receiver
+            call_type = CallType.CALL
+
         evm_call = get_calltree_from_geth_trace(
             self._get_transaction_trace(txn_hash),
             gas_cost=method_gas_cost,
             gas_limit=receipt.gas_limit,
-            address=receipt.receiver,
+            address=address,
             calldata=receipt.data,
             value=receipt.value,
-            call_type=CallType.CALL,
+            call_type=call_type,
             failed=receipt.failed,
         )
         # Strange bug in Ganache where sub-calls REVERT trickles to the top-level
         # CALL when it is not supposed to. Reset `failed`.
         evm_call.failed = receipt.failed
 
         return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
```

### Comparing `ape-ganache-0.6.7/ape_ganache.egg-info/PKG-INFO` & `ape-ganache-0.6.8/ape_ganache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ganache
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-ganache: Ape network provider for Ganache
 Home-page: https://github.com/ApeWorX/ape-ganache
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ganache-0.6.7/ape_ganache.egg-info/SOURCES.txt` & `ape-ganache-0.6.8/ape_ganache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/ape_ganache.egg-info/requires.txt` & `ape-ganache-0.6.8/ape_ganache.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/pyproject.toml` & `ape-ganache-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/setup.py` & `ape-ganache-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/ape-config.yaml` & `ape-ganache-0.6.8/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/conftest.py` & `ape-ganache-0.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_a.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_b.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/contract_c.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/has_error.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/token_a.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/token_b.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-ganache-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/python/pytest_tests.py` & `ape-ganache-0.6.8/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/sources/TokenA.vy` & `ape-ganache-0.6.8/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/data/sources/TokenB.vy` & `ape-ganache-0.6.8/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/expected_traces.py` & `ape-ganache-0.6.8/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/test_fork_provider.py` & `ape-ganache-0.6.8/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/test_gas_report.py` & `ape-ganache-0.6.8/tests/test_gas_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,33 @@
 TEST_FILE = (BASE_DATA_PATH / "pytest_tests.py").read_text()
 NUM_TESTS = len([x for x in TEST_FILE.split("\n") if x.startswith("def test_")])
 TOKEN_B_GAS_REPORT = r"""
  +TokenB Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
+  __init__ +\d +\d+ + \d+ + \d+ + \d+
   balanceOf +\d +\d+ + \d+ + \d+ + \d+
   transfer +\d +\d+ + \d+ + \d+ + \d+
 """
 EXPECTED_GAS_REPORT = rf"""
  +TestContractVy Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
+  __init__ +\d +\d+ + \d+ + \d+ + \d+
+  fooAndBar +\d +\d+ + \d+ + \d+ + \d+
   myNumber +\d +\d+ + \d+ + \d+ + \d+
   setNumber +\d +\d+ + \d+ + \d+ + \d+
-  fooAndBar +\d +\d+ + \d+ + \d+ + \d+
 
  +TokenA Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
+  __init__ +\d +\d+ + \d+ + \d+ + \d+
   balanceOf +\d +\d+ + \d+ + \d+ + \d+
   transfer +\d +\d+ + \d+ + \d+ + \d+
 {TOKEN_B_GAS_REPORT}
 """
 
 
 def filter_expected_methods(expected, *methods_to_remove: str) -> str:
```

### Comparing `ape-ganache-0.6.7/tests/test_provider.py` & `ape-ganache-0.6.8/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.7/tests/test_trace.py` & `ape-ganache-0.6.8/tests/test_trace.py`

 * *Files identical despite different names*


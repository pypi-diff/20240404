# Comparing `tmp/bowtie_json_schema-2024.3.9.tar.gz` & `tmp/bowtie_json_schema-2024.4.1.tar.gz`

## Comparing `bowtie_json_schema-2024.3.9.tar` & `bowtie_json_schema-2024.4.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.prettierrc.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/action.yml
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/noxfile.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/test-requirements.in
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/test-requirements.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.devcontainer/.codespace.Dockerfile
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/__main__.py
--rw-r--r--   0        0        0    42570 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_cli.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_containers.py
--rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_core.py
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_report.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/exceptions.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/py.typed
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/Makefile
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/cli.rst
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/github-actions.rst
--rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/motd.txt
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/requirements.in
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/package.json
--rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/global.css
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/conftest.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_implementation.py
--rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_integration.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_report.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/hatch_build.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.prettierrc.json
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/action.yml
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/noxfile.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/test-requirements.in
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/test-requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.devcontainer/Containerfile
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/__main__.py
+-rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_cli.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_containers.py
+-rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_core.py
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_report.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/py.typed
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/github-actions.rst
+-rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/requirements.in
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/index.html
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/package.json
+-rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_github.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_implementation.py
+-rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_integration.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_report.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/hatch_build.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.3.9/.gitpod.yml` & `bowtie_json_schema-2024.4.1/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/.pre-commit-config.yaml` & `bowtie_json_schema-2024.4.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.4"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.1
     hooks:
       - name: ensure bowtie's own schemas are valid
         id: check-metaschema
         files: ^bowtie/schemas/.*\.json$
   - repo: local
     hooks:
       - id: check-dependabot
```

### Comparing `bowtie_json_schema-2024.3.9/CONTRIBUTING.rst` & `bowtie_json_schema-2024.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/action.yml` & `bowtie_json_schema-2024.4.1/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/noxfile.py` & `bowtie_json_schema-2024.4.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/requirements.txt` & `bowtie_json_schema-2024.4.1/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     #   rich
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pygments==2.17.2
     # via
     #   jsonschema-lexer
     #   rich
 pyjwt==2.8.0
     # via github3-py
```

### Comparing `bowtie_json_schema-2024.3.9/test-requirements.txt` & `bowtie_json_schema-2024.4.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_cli.py` & `bowtie_json_schema-2024.4.1/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import json
 import logging
 import os
 import sys
 
 from aiodocker import Docker
 from attrs import asdict
+from click.shell_completion import CompletionItem
 from diagnostic import DiagnosticError
 from jsonschema_lexer import JSONSchemaLexer
 from pygments.lexers.data import (  # type: ignore[reportMissingTypeStubs]
     JsonLexer,
 )
 from referencing.jsonschema import EMPTY_REGISTRY
 from rich import box, console, panel
@@ -657,14 +658,26 @@
         param: click.Parameter | None,
         ctx: click.Context | None,
     ) -> str:
         if "/" in value:  # a fully qualified image name
             return value
         return f"{IMAGE_REPOSITORY}/{value}"
 
+    def shell_complete(
+        self,
+        ctx: click.Context,
+        param: click.Parameter,
+        incomplete: str,
+    ) -> list[CompletionItem]:
+        return [
+            CompletionItem(name)
+            for name in Implementation.known()
+            if name.startswith(incomplete.lower())
+        ]
+
 
 class _Dialect(click.ParamType):
     """
     Select a JSON Schema dialect.
     """
 
     name = "dialect"
@@ -689,14 +702,44 @@
         else:
             dialect = Dialect.by_uri().get(url)
             if dialect is not None:
                 return dialect
 
         self.fail(f"{value!r} is not a known dialect URI or short name.")
 
+    def shell_complete(
+        self,
+        ctx: click.Context,
+        param: click.Parameter,
+        incomplete: str,
+    ) -> list[CompletionItem]:
+        if incomplete:  # the user typed something, so filter over everything
+            suggestions = [
+                (field, dialect)
+                for dialect in Dialect.known()
+                for field in [
+                    str(dialect.uri),
+                    dialect.short_name,
+                    *dialect.aliases,
+                ]
+            ]
+            suggestions = [(str(u), d) for u, d in Dialect.by_uri().items()]
+        else:  # the user didn't type anything, only suggest short names
+            suggestions = Dialect.by_short_name().items()
+
+        return [
+            # FIXME: pallets/click#2703
+            CompletionItem(
+                value=value.replace(":", "\\:"),
+                help=f"the {dialect.pretty_name} dialect",
+            )
+            for value, dialect in suggestions
+            if value.startswith(incomplete.lower())
+        ]
+
 
 CaseTransform = Callable[[Iterable[TestCase]], Iterable[TestCase]]
 
 
 class _Filter(click.ParamType):
     """
     Filter some test cases by a pattern.
@@ -985,15 +1028,15 @@
     dialects: Sequence[Dialect],
     languages: Set[str],
 ):
     """
     Output implementations matching a given criteria.
     """
     if not dialects and languages == KNOWN_LANGUAGES:
-        for implementation in ctx.params["image_names"]:
+        for implementation in ctx.params.get("image_names", ()):
             click.echo(implementation.removeprefix(f"{IMAGE_REPOSITORY}/"))
         return
 
     async for each in start():
         if each.supports(*dialects) and each.info.language in languages:
             click.echo(each.name.removeprefix(f"{IMAGE_REPOSITORY}/"))
```

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_commands.py` & `bowtie_json_schema-2024.4.1/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_containers.py` & `bowtie_json_schema-2024.4.1/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_core.py` & `bowtie_json_schema-2024.4.1/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_report.py` & `bowtie_json_schema-2024.4.1/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/_suite.py` & `bowtie_json_schema-2024.4.1/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/exceptions.py` & `bowtie_json_schema-2024.4.1/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/hypothesis.py` & `bowtie_json_schema-2024.4.1/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.4.1/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/data/dialects.json` & `bowtie_json_schema-2024.4.1/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/Makefile` & `bowtie_json_schema-2024.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/cli.rst` & `bowtie_json_schema-2024.4.1/docs/cli.rst`

 * *Files 19% similar despite different names*

```diff
@@ -94,13 +94,89 @@
 E.g., to verify the Golang ``jsonschema`` implementation is functioning, you can run:
 
 .. code:: sh
 
    $ bowtie smoke -i go-jsonschema
 
 
+Enabling Shell Tab Completion
+-----------------------------
+
+The Bowtie CLI supports tab completion using the `click module's built-in support <click:shell-completion>`.
+Below are short instructions for your shell using the default configuration paths.
+
+.. tabs::
+    .. group-tab:: Bash
+
+        Add this to ``~/.bashrc``:
+
+        .. code:: sh
+
+            $ eval "$(_BOWTIE_COMPLETE=bash_source bowtie)"
+
+    .. group-tab:: Zsh
+
+        Add this to ``~/.zshrc``:
+
+        .. code:: sh
+
+            $ eval "$(_BOWTIE_COMPLETE=zsh_source bowtie)"
+
+    .. group-tab:: Fish
+
+        Add this to ``~/.config/fish/completions/bowtie.fish``:
+
+        .. code:: sh
+
+            $ _BOWTIE_COMPLETE=fish_source bowtie | source
+
+        This is the same file used for the activation script method below. For Fish it's probably always easier to use that method.
+
+Using ``eval`` means that the command is invoked and evaluated every time a shell is started, which can delay shell responsiveness.
+To speed it up, write the generated script to a file, then source that.
+
+.. tabs::
+    .. group-tab:: Bash
+
+        Save the script somewhere.
+
+        .. code:: sh
+
+            $ _BOWTIE_COMPLETE=bash_source bowtie > ~/.bowtie-complete.bash
+
+        Source the file in ``~/.bashrc``.
+
+        .. code:: sh
+
+            $ . ~/.bowtie-complete.bash
+
+    .. group-tab:: Zsh
+
+        Save the script somewhere.
+
+        .. code:: sh
+
+            $ _BOWTIE_COMPLETE=zsh_source bowtie > ~/.bowtie-complete.zsh
+
+        Source the file in ``~/.zshrc``.
+
+        .. code:: sh
+
+            $ . ~/.bowtie-complete.zsh
+
+    .. group-tab:: Fish
+
+        Save the script to ``~/.config/fish/completions/bowtie.fish``:
+
+        .. code:: sh
+
+            $ _BOWTIE_COMPLETE=fish_source bowtie > ~/.config/fish/completions/bowtie.fish
+
+After modifying your shell configuration, you may need to start a new shell in order for the changes to be loaded.
+
+
 Reference
 ---------
 
 .. click:: bowtie._cli:main
    :prog: bowtie
    :nested: full
```

### Comparing `bowtie_json_schema-2024.3.9/docs/conf.py` & `bowtie_json_schema-2024.4.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "sphinx.ext.doctest",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx_click",
     "sphinx_copybutton",
+    "sphinx_tabs.tabs",
     "sphinx_json_schema_spec",
     "sphinx_substitution_extensions",
     "sphinxcontrib.spelling",
     "sphinxext.opengraph",
 ]
 
 pygments_style = "lovelace"
@@ -120,17 +121,18 @@
 # -- autosectionlabel --
 
 autosectionlabel_prefix_document = True
 
 # -- intersphinx --
 
 intersphinx_mapping = {
+    "click": ("https://click.palletsprojects.com", None),
     "nox": ("https://nox.thea.codes/en/stable/", None),
-    "podman": ("https://docs.podman.io/en/latest", None),
     "pip": ("https://pip.pypa.io/en/stable/", None),
+    "podman": ("https://docs.podman.io/en/latest", None),
     "python": ("https://docs.python.org/", None),
     "sphinx": ("https://www.sphinx-doc.org", None),
 }
 
 # -- extlinks --
 
 extlinks = {
```

### Comparing `bowtie_json_schema-2024.3.9/docs/contributing.rst` & `bowtie_json_schema-2024.4.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/github-actions.rst` & `bowtie_json_schema-2024.4.1/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/implementers.rst` & `bowtie_json_schema-2024.4.1/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/index.rst` & `bowtie_json_schema-2024.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/motd.txt` & `bowtie_json_schema-2024.4.1/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/docs/requirements.txt` & `bowtie_json_schema-2024.4.1/docs/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 docutils==0.20.1
     # via
     #   diagnostic
     #   sphinx
     #   sphinx-click
     #   sphinx-prompt
     #   sphinx-substitution-extensions
+    #   sphinx-tabs
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 furo==2024.1.29
     # via -r docs/requirements.in
 github3-py==4.0.1
@@ -91,14 +92,15 @@
     # via
     #   furo
     #   jsonschema-lexer
     #   pygments-github-lexers
     #   rich
     #   sphinx
     #   sphinx-prompt
+    #   sphinx-tabs
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
 pyjwt==2.8.0
     # via github3-py
 python-dateutil==2.9.0.post0
     # via github3-py
 referencing==0.34.0
@@ -134,28 +136,31 @@
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
     #   sphinx-prompt
     #   sphinx-substitution-extensions
+    #   sphinx-tabs
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==5.1.0
     # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
 sphinx-json-schema-spec==2024.1.1
     # via -r docs/requirements.in
 sphinx-prompt==1.8.0
     # via sphinx-substitution-extensions
 sphinx-substitution-extensions==2024.2.25
     # via -r docs/requirements.in
+sphinx-tabs==3.4.5
+    # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
```

### Comparing `bowtie_json_schema-2024.3.9/docs/_static/logo.svg` & `bowtie_json_schema-2024.4.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/package.json` & `bowtie_json_schema-2024.4.1/frontend/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9486842105263158%*

 * *Differences: {"'devDependencies'": "{'vite': '^5.1.7'}", "'packageManager'": "'pnpm@8.15.1'"}*

```diff
@@ -24,15 +24,15 @@
         "eslint-plugin-react": "7.33.2",
         "eslint-plugin-react-hooks": "4.6.0",
         "jsdom": "^24.0.0",
         "react-test-renderer": "^18.2.0",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
         "typescript": "^5.3.3",
-        "vite": "^5.1.1",
+        "vite": "^5.1.7",
         "vite-bundle-visualizer": "^1.1.0",
         "vitest": "^1.3.1"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
@@ -70,15 +70,15 @@
         "settings": {
             "react": {
                 "version": "18.2"
             }
         }
     },
     "name": "bowtie",
-    "packageManager": "pnpm@8.x",
+    "packageManager": "pnpm@8.15.1",
     "scripts": {
         "build": "tsc && vite build",
         "bundle-visualizer": "vite-bundle-visualizer",
         "lint": "eslint src --max-warnings 0",
         "preview": "vite preview",
         "start": "vite --no-clearScreen",
         "test": "vitest run",
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.4.1/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     specifier: ^7.0.0
     version: 7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.56.0)(typescript@5.3.3)
   '@typescript-eslint/parser':
     specifier: ^6.21.0
     version: 6.21.0(eslint@8.56.0)(typescript@5.3.3)
   '@vitejs/plugin-react':
     specifier: ^4.2.1
-    version: 4.2.1(vite@5.1.1)
+    version: 4.2.1(vite@5.1.7)
   eslint:
     specifier: 8.56.0
     version: 8.56.0
   eslint-plugin-react:
     specifier: 7.33.2
     version: 7.33.2(eslint@8.56.0)
   eslint-plugin-react-hooks:
@@ -79,16 +79,16 @@
   ts-node:
     specifier: ^10.9.2
     version: 10.9.2(@types/node@20.11.5)(typescript@5.3.3)
   typescript:
     specifier: ^5.3.3
     version: 5.3.3
   vite:
-    specifier: ^5.1.1
-    version: 5.1.1(@types/node@20.11.5)
+    specifier: ^5.1.7
+    version: 5.1.7(@types/node@20.11.5)
   vite-bundle-visualizer:
     specifier: ^1.1.0
     version: 1.1.0
   vitest:
     specifier: ^1.3.1
     version: 1.3.1(@types/node@20.11.5)(jsdom@24.0.0)
 
@@ -1141,26 +1141,26 @@
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@ungap/structured-clone@1.2.0:
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
     dev: true
 
-  /@vitejs/plugin-react@4.2.1(vite@5.1.1):
+  /@vitejs/plugin-react@4.2.1(vite@5.1.7):
     resolution: {integrity: sha512-oojO9IDc4nCUUi8qIR11KoQm0XFFLIwsRBwHRR4d/88IWghn1y6ckz/bJ8GHDCsYEJee8mDzqtJxh15/cisJNQ==}
     engines: {node: ^14.18.0 || >=16.0.0}
     peerDependencies:
       vite: ^4.2.0 || ^5.0.0
     dependencies:
       '@babel/core': 7.23.7
       '@babel/plugin-transform-react-jsx-self': 7.23.3(@babel/core@7.23.7)
       '@babel/plugin-transform-react-jsx-source': 7.23.3(@babel/core@7.23.7)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.0
-      vite: 5.1.1(@types/node@20.11.5)
+      vite: 5.1.7(@types/node@20.11.5)
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@vitest/expect@1.3.1:
     resolution: {integrity: sha512-xofQFwIzfdmLLlHa6ag0dPV8YsnKOCP1KdAeVVh34vSjN2dcUiXYCD9htu/9eM7t8Xln4v03U9HLxLpPlsXdZw==}
     dependencies:
@@ -4086,28 +4086,28 @@
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       pathe: 1.1.2
       picocolors: 1.0.0
-      vite: 5.1.1(@types/node@20.11.5)
+      vite: 5.1.7(@types/node@20.11.5)
     transitivePeerDependencies:
       - '@types/node'
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
     dev: true
 
-  /vite@5.1.1(@types/node@20.11.5):
-    resolution: {integrity: sha512-wclpAgY3F1tR7t9LL5CcHC41YPkQIpKUGeIuT8MdNwNZr6OqOTLs7JX5vIHAtzqLWXts0T+GDrh9pN2arneKqg==}
+  /vite@5.1.7(@types/node@20.11.5):
+    resolution: {integrity: sha512-sgnEEFTZYMui/sTlH1/XEnVNHMujOahPLGMxn1+5sIT45Xjng1Ec1K78jRP15dSmVgg5WBin9yO81j3o9OxofA==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
@@ -4178,15 +4178,15 @@
       magic-string: 0.30.7
       pathe: 1.1.2
       picocolors: 1.0.0
       std-env: 3.7.0
       strip-literal: 2.0.0
       tinybench: 2.6.0
       tinypool: 0.8.2
-      vite: 5.1.1(@types/node@20.11.5)
+      vite: 5.1.7(@types/node@20.11.5)
       vite-node: 1.3.1(@types/node@20.11.5)
       why-is-node-running: 2.2.2
     transitivePeerDependencies:
       - less
       - lightningcss
       - sass
       - stylus
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/tsconfig.json` & `bowtie_json_schema-2024.4.1/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/public/favicon.svg` & `bowtie_json_schema-2024.4.1/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/index.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/index.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,20 @@
   const promises = [];
   for (const dialect of Dialect.known()) {
     promises.push(
       dialect.fetchReport().then((data) => allReportsData.set(dialect, data)),
     );
   }
   await Promise.all(promises);
-  return prepareImplementationReport(allReportsData, langImplementation);
+
+  // FIXME: This magic prefix is duplicated from the backend side,
+  //        and probably we can separate handling this in Implementation
+  //        class (when we have it).
+  const implementationId = `ghcr.io/bowtie-json-schema/${langImplementation}`;
+  return prepareImplementationReport(allReportsData, implementationId);
 };
 
 const fetchImplementationMetadata = async () => {
   const response = await fetch(implementationMetadataURI);
   const implementations = (await response.json()) as Record<
     string,
     ImplementationData
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.4.1/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/CopyToClipboard.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import { useState } from "react";
-import { Check, Copy } from "react-bootstrap-icons";
-import Button from "react-bootstrap/Button";
+import { CheckLg, Copy } from "react-bootstrap-icons";
 import OverlayTrigger from "react-bootstrap/OverlayTrigger";
 import Tooltip from "react-bootstrap/Tooltip";
 
 interface CopyProps {
   textToCopy: string;
   style?: string;
 }
@@ -30,16 +29,20 @@
         placement="top"
         overlay={
           <Tooltip id="tooltip-top">
             {copied ? "Copied!" : "Copy to clipboard"}
           </Tooltip>
         }
       >
-        <Button variant="dark" className={style} onClick={handleCopy}>
-          {copied ? <Check /> : <Copy />}
-        </Button>
+        <div
+          className={style}
+          onClick={handleCopy}
+          style={{ cursor: "pointer" }}
+        >
+          {copied ? <CheckLg className="text-success" /> : <Copy />}
+        </div>
       </OverlayTrigger>
     </>
   );
 }
 
 export default CopyToClipboard;
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/NavBar.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-import { useContext, useEffect } from "react";
+import { useContext, useEffect, useState } from "react";
 import { Sun, MoonStarsFill, Book } from "react-bootstrap-icons";
 import { Link, useLocation, useMatch } from "react-router-dom";
+import Container from "react-bootstrap/Container";
+import Navbar from "react-bootstrap/Navbar";
 import NavDropdown from "react-bootstrap/NavDropdown";
+import Collapse from "react-bootstrap/Collapse";
 
 import { ThemeContext } from "../context/ThemeContext";
 import { BowtieVersionContext } from "../context/BowtieVersionContext";
 import logo from "../assets/landscape-logo.svg";
 import Dialect from "../data/Dialect";
 
 const NavBar = () => {
   const { isDarkMode, toggleDarkMode } = useContext(ThemeContext);
   const { version } = useContext(BowtieVersionContext);
   const { hash, key } = useLocation();
+  const [isNavbarOpen, setIsNavbarOpen] = useState(false);
 
   const rootMatch = useMatch("/");
   const dialectsMatch = useMatch("/dialects/*");
   const isDialectPage = rootMatch ?? dialectsMatch;
 
   useEffect(() => {
     if (hash) {
       const targetElement = document.getElementById(hash.substring(1));
       targetElement?.scrollIntoView({ behavior: "smooth" });
     }
   }, [key, hash]);
 
   return (
-    <>
-      <nav
-        className={`navbar navbar-expand-lg sticky-top mb-4 ${
-          isDarkMode ? "navbar-dark bg-dark" : "navbar-light bg-light"
-        }`}
+    <Navbar
+      expand="lg"
+      sticky="top"
+      className={`mb-4 ${
+        isDarkMode ? "navbar-dark bg-dark" : "navbar-light bg-light"
+      }`}
+    >
+      <Container
+        fluid
+        className="d-flex justify-content-between align-items-center"
       >
-        <div className="container-fluid d-flex justify-content-between align-items-center">
-          <Link className="navbar-brand me-4 py-1" to="/">
-            <img src={logo} alt="Bowtie Logo" width="128px" />
-          </Link>
-          <div className="d-flex align-items-center">
-            <div className="d-lg-none d-flex justify-content-between align-items-center me-2">
-              <Link
-                className="nav-link border border-primary rounded-3 d-inline-block p-2 me-1"
-                to="https://docs.bowtie.report/"
-                target="_blank"
-              >
-                <Book size={20} />
-              </Link>
-              <button
-                className={`btn d-flex align-items-center justify-content-center ${
-                  isDarkMode ? "btn-light" : "btn-secondary"
-                } rounded me-1 p-2`}
-                onClick={() => toggleDarkMode!()}
-              >
-                {isDarkMode ? <MoonStarsFill size={20} /> : <Sun size={20} />}
-              </button>
-            </div>
+        <Link className="navbar-brand me-4 py-1" to="/">
+          <img src={logo} alt="Bowtie Logo" width="128px" />
+        </Link>
+        <div className="d-flex align-items-center">
+          <div className="d-lg-none d-flex justify-content-between align-items-center me-2">
+            <Link
+              className="nav-link border border-primary rounded-3 d-inline-block p-2 me-1"
+              to="https://docs.bowtie.report/"
+              target="_blank"
+            >
+              <Book size={20} />
+            </Link>
             <button
-              className="navbar-toggler"
               type="button"
-              data-bs-toggle="collapse"
-              data-bs-target="#navbarNav"
-              aria-controls="navbarSupportedContent"
-              aria-expanded="false"
-              aria-label="Toggle navigation"
+              className={`btn d-flex align-items-center justify-content-center ${
+                isDarkMode ? "btn-light" : "btn-secondary"
+              } rounded me-1 p-2`}
+              onClick={() => toggleDarkMode!()}
             >
-              <span className="navbar-toggler-icon"></span>
+              {isDarkMode ? <MoonStarsFill size={20} /> : <Sun size={20} />}
             </button>
           </div>
-          <div className="collapse navbar-collapse" id="navbarNav">
+          <Navbar.Toggle
+            aria-controls="collapse-navbar-nav"
+            aria-expanded="false"
+            aria-label="Toggle navigation"
+            onClick={() => setIsNavbarOpen(!isNavbarOpen)}
+          />
+        </div>
+        <Collapse in={isNavbarOpen}>
+          <div className="collapse navbar-collapse" id="navbarSupportedContent">
             <ul className="navbar-nav me-auto mb-2 mb-lg-0 align-items-baseline">
               {isDialectPage && (
                 <>
                   <li className="nav-item">
                     <Link className="nav-link" to={{ hash: "run-info" }}>
                       Run Info
                     </Link>
@@ -82,15 +87,15 @@
                   <li className="nav-item">
                     <Link className="nav-link" to={{ hash: "cases" }}>
                       Details
                     </Link>
                   </li>
                 </>
               )}
-              <NavDropdown id="dialect-dropdown" title="Dialects">
+              <NavDropdown title="Dialects" id="dialect-dropdown">
                 {Dialect.newest_to_oldest().map((dialect) => (
                   <NavDropdown.Item
                     as={Link}
                     to={dialect.routePath}
                     key={dialect.shortName}
                   >
                     {dialect.prettyName}
@@ -111,40 +116,41 @@
                   <span className="navbar-text">
                     {version && `Bowtie v ${version}`}
                   </span>
                 </a>
               </li>
             </ul>
           </div>
-          <div className="large-screen d-none d-lg-block">
-            <Link
-              className="nav-link border border-primary rounded-3 me-1 d-inline-block text-center py-2 px-3"
-              to="https://docs.bowtie.report/"
-              target="_blank"
-            >
-              <Book size={20} className="me-1" />
-              Docs
-            </Link>
-            <button
-              className="btn border-0 me-1"
-              onClick={() => toggleDarkMode!()}
-            >
-              {isDarkMode ? <MoonStarsFill size={20} /> : <Sun size={20} />}
-            </button>
-            <a
-              href="https://github.com/bowtie-json-schema/bowtie/"
-              className="link-secondary"
-              rel="noopener noreferrer"
-              target="_blank"
-            >
-              <span className="navbar-text">
-                {version && <small>Bowtie v{version}</small>}
-              </span>
-            </a>
-          </div>
+        </Collapse>
+        <div className="large-screen d-none d-lg-block">
+          <Link
+            className="nav-link border border-primary rounded-3 me-1 d-inline-block text-center py-2 px-3"
+            to="https://docs.bowtie.report/"
+            rel="noopener noreferrer"
+            target="_blank"
+          >
+            <Book size={20} className="me-1" />
+            Docs
+          </Link>
+          <button
+            className="btn border-0 me-1"
+            onClick={() => toggleDarkMode!()}
+          >
+            {isDarkMode ? <MoonStarsFill size={20} /> : <Sun size={20} />}
+          </button>
+          <a
+            href="https://github.com/bowtie-json-schema/bowtie/"
+            className="link-secondary"
+            rel="noopener noreferrer"
+            target="_blank"
+          >
+            <span className="navbar-text">
+              {version && <small>Bowtie v{version}</small>}
+            </span>
+          </a>
         </div>
-      </nav>
-    </>
+      </Container>
+    </Navbar>
   );
 };
 
 export default NavBar;
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import { useContext } from "react";
 import CopyToClipboard from "../CopyToClipboard";
 import { Prism as SyntaxHighlighter } from "react-syntax-highlighter";
-import { atomDark } from "react-syntax-highlighter/dist/esm/styles/prism";
+import {
+  oneLight,
+  oneDark,
+} from "react-syntax-highlighter/dist/esm/styles/prism";
+import { ThemeContext } from "../../context/ThemeContext";
 
 const SchemaDisplay = ({
   schema,
   instance,
 }: {
   instance: unknown;
   schema: Record<string, unknown> | boolean;
 }) => {
+  const { isDarkMode } = useContext(ThemeContext);
   const schemaFormatted = JSON.stringify(schema, null, 2);
   const instanceFormatted = JSON.stringify(instance, null, 2);
   return (
     <div className="card mb-3 mw-100">
       <div className="d-flex">
         <div className="col-md-8 col-6 pe-0">
           <div className="d-flex align-items-center highlight-toolbar ps-3 pe-2 py-1 border-0 border-top border-bottom">
@@ -20,34 +26,40 @@
               Schema
             </small>
             <div className="d-flex ms-auto"></div>
           </div>
           <div className="card-body position-relative">
             <CopyToClipboard
               textToCopy={schemaFormatted}
-              style="position-absolute top-0 end-0 mt-4 me-3"
+              style="position-absolute top-0 end-0 mt-4 me-4"
             />
-            <SyntaxHighlighter language="json" style={atomDark}>
+            <SyntaxHighlighter
+              language="json"
+              style={isDarkMode ? oneDark : oneLight}
+            >
               {schemaFormatted}
             </SyntaxHighlighter>
           </div>
         </div>
         <div className="col-md-4 col-6 border-start px-0">
           <div className="d-flex align-items-center highlight-toolbar ps-3 pe-2 py-1 border-0 border-top border-bottom">
             <small className="font-monospace text-body-secondary text-uppercase pe-4">
               Instance
             </small>
             <div className="d-flex ms-auto"></div>
           </div>
           <div id="instance-info" className="card-body position-relative">
             <CopyToClipboard
               textToCopy={instanceFormatted}
-              style="position-absolute top-0 end-0 mt-4 me-3"
+              style="position-absolute top-0 end-0 mt-4 me-4"
             />
-            <SyntaxHighlighter language="json" style={atomDark}>
+            <SyntaxHighlighter
+              language="json"
+              style={isDarkMode ? oneDark : oneLight}
+            >
               {instanceFormatted}
             </SyntaxHighlighter>
           </div>
         </div>
       </div>
     </div>
   );
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.4.1/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.test.ts`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 import { mkdtemp, rm, writeFile } from "node:fs/promises";
 import { spawnSync } from "node:child_process";
 import { tmpdir } from "node:os";
 
 import { describe, expect, test } from "vitest";
 
 import Dialect from "./Dialect";
-import { RunMetadata, fromSerialized } from "./parseReportData";
+import {
+  RunMetadata,
+  ReportData,
+  fromSerialized,
+  prepareImplementationReport,
+} from "./parseReportData";
 
 function tag(image: string) {
   // Should match what's used in our `noxfile`, certainly until we handle image
   // building here from the frontend test suite.
   return `bowtie-ui-tests/${image}`;
 }
 
@@ -35,14 +40,80 @@
         ${result.stderr?.toString()}
     `;
     throw error;
   }
   return result.stdout.toString();
 }
 
+const testCases = {
+  case1: {
+    description: "case1",
+    schema: {
+      additionalProperties: { type: "boolean" },
+      properties: { bar: {}, foo: {} },
+    },
+    tests: [
+      {
+        description: "one",
+        instance: { foo: 1 },
+        valid: true,
+      },
+      {
+        description: "two",
+        instance: { foo: 1, bar: 2, quux: true },
+        valid: true,
+      },
+      {
+        description: "three",
+        instance: { foo: 1, bar: 2, quux: 12 },
+        valid: false,
+      },
+    ],
+  },
+  case2: {
+    description: "case2",
+    schema: {
+      additionalProperties: { type: "boolean" },
+    },
+    tests: [
+      {
+        description: "one",
+        instance: { foo: true },
+        valid: true,
+      },
+      {
+        description: "two",
+        instance: { foo: 1 },
+        valid: false,
+      },
+    ],
+  },
+  case3: {
+    description: "case3",
+    schema: {
+      allOf: [
+        { $ref: "https://example.com/schema-with-anchor#foo" },
+        { then: { $id: "http://example.com/ref/then", type: "integer" } },
+      ],
+    },
+    tests: [
+      {
+        description: "one",
+        instance: "foo",
+        valid: false,
+      },
+      {
+        description: "two",
+        instance: 12,
+        valid: true,
+      },
+    ],
+  },
+};
+
 describe("parseReportData", () => {
   test("parses reports", async () => {
     let lines: string;
 
     const tempdir = await mkdtemp(join(tmpdir(), "bowtie-ui-tests-"));
 
     try {
@@ -116,78 +187,15 @@
         ],
       ]),
       didFailFast: false,
     });
   });
 
   test("parses reports with multiple test cases", () => {
-    const case1 = {
-      description: "case1",
-      schema: {
-        additionalProperties: { type: "boolean" },
-        properties: { bar: {}, foo: {} },
-      },
-      tests: [
-        {
-          description: "one",
-          instance: { foo: 1 },
-          valid: true,
-        },
-        {
-          description: "two",
-          instance: { foo: 1, bar: 2, quux: true },
-          valid: true,
-        },
-        {
-          description: "three",
-          instance: { foo: 1, bar: 2, quux: 12 },
-          valid: false,
-        },
-      ],
-    };
-    const case2 = {
-      description: "case2",
-      schema: {
-        additionalProperties: { type: "boolean" },
-      },
-      tests: [
-        {
-          description: "one",
-          instance: { foo: true },
-          valid: true,
-        },
-        {
-          description: "two",
-          instance: { foo: 1 },
-          valid: false,
-        },
-      ],
-    };
-    const case3 = {
-      description: "case3",
-      schema: {
-        allOf: [
-          { $ref: "https://example.com/schema-with-anchor#foo" },
-          { then: { $id: "http://example.com/ref/then", type: "integer" } },
-        ],
-      },
-      tests: [
-        {
-          description: "one",
-          instance: "foo",
-          valid: false,
-        },
-        {
-          description: "two",
-          instance: 12,
-          valid: true,
-        },
-      ],
-    };
-    const cases = [case1, case2, case3].map((each) => JSON.stringify(each));
+    const cases = Object.values(testCases).map((each) => JSON.stringify(each));
 
     const lines = bowtie(
       ["run", "-i", tag("envsonschema"), "-D", "7"],
       cases.join("\n") + "\n",
     );
 
     const report = fromSerialized(lines);
@@ -254,33 +262,92 @@
           },
         ],
       ]),
       cases: new Map([
         [
           1,
           {
-            description: case1.description,
-            schema: case1.schema,
-            tests: case1.tests,
+            description: testCases.case1.description,
+            schema: testCases.case1.schema,
+            tests: testCases.case1.tests,
           },
         ],
         [
           2,
           {
-            description: case2.description,
-            schema: case2.schema,
-            tests: case2.tests,
+            description: testCases.case2.description,
+            schema: testCases.case2.schema,
+            tests: testCases.case2.tests,
           },
         ],
         [
           3,
           {
-            description: case3.description,
-            schema: case3.schema,
-            tests: case3.tests,
+            description: testCases.case3.description,
+            schema: testCases.case3.schema,
+            tests: testCases.case3.tests,
           },
         ],
       ]),
       didFailFast: false,
     });
   });
+
+  test("prepares a summarized implementation report using all the dialect reports", () => {
+    const cases = Object.values(testCases).map((each) => JSON.stringify(each));
+    const allReportsData = new Map<Dialect, ReportData>();
+
+    for (const dialect of Dialect.known()) {
+      const lines = bowtie(
+        ["run", "-i", tag("envsonschema"), "-D", dialect.shortName],
+        cases.join("\n") + "\n",
+      );
+      const report = fromSerialized(lines);
+      allReportsData.set(dialect, report);
+    }
+
+    const implementationReport = prepareImplementationReport(
+      allReportsData,
+      tag("envsonschema"),
+    );
+
+    const metadata = implementationReport!.implementation;
+
+    expect(implementationReport).toStrictEqual({
+      implementation: {
+        name: "envsonschema",
+        language: "python",
+        homepage: metadata.homepage,
+        issues: metadata.issues,
+        source: metadata.source,
+        dialects: metadata.dialects,
+        links: metadata.links,
+      },
+      dialectCompliance: new Map([
+        [
+          Dialect.withName("draft2020-12"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+        [
+          Dialect.withName("draft2019-09"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+        [
+          Dialect.withName("draft7"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+        [
+          Dialect.withName("draft6"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+        [
+          Dialect.withName("draft4"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+        [
+          Dialect.withName("draft3"),
+          { erroredTests: 0, skippedTests: 0, failedTests: 4 },
+        ],
+      ]),
+    });
+  });
 });
```

### Comparing `bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.ts`

 * *Files 2% similar despite different names*

```diff
@@ -172,44 +172,39 @@
 ): Implementation =>
   ({
     ...data,
     dialects: data.dialects.map((uri) => Dialect.forURI(uri)),
   }) as Implementation;
 
 /**
- * Prepare a summarized implementation report for the
- * passed implementation using all the dialect reports data
+ * Prepare a summarized implementation report using the
+ * passed implementation id and all the dialect reports data
  * that was fetched.
  */
 export const prepareImplementationReport = (
   allReportsData: Map<Dialect, ReportData>,
-  langImplementation: string,
+  implementationId: string,
 ) => {
   let implementationReport: ImplementationReport | null = null;
   const dialectCompliance = new Map<Dialect, Partial<Totals>>();
 
-  // FIXME: This magic prefix is duplicated from the backend side,
-  //        and probably we can separate handling this in Implementation
-  //        class (when we have it).
-  const image = `ghcr.io/bowtie-json-schema/${langImplementation}`;
-
   for (const [
     dialect,
     { implementationsResults, runMetadata },
   ] of allReportsData.entries()) {
-    const implementationResults = implementationsResults.get(image);
+    const implementationResults = implementationsResults.get(implementationId);
 
     if (implementationResults) {
       dialectCompliance.set(dialect, {
         erroredTests: implementationResults.totals.erroredTests,
         skippedTests: implementationResults.totals.skippedTests,
         failedTests: implementationResults.totals.failedTests,
       });
 
-      const implementation = runMetadata.implementations.get(image)!;
+      const implementation = runMetadata.implementations.get(implementationId)!;
 
       if (!implementationReport) {
         implementationReport = {
           implementation,
           dialectCompliance,
         };
       } else {
```

### Comparing `bowtie_json_schema-2024.3.9/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.4.1/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.4.1/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.4.1/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.4.1/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.4.1/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.4.1/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.4.1/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.4.1/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.4.1/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.4.1/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.4.1/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.4.1/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.4.1/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_cli.py` & `bowtie_json_schema-2024.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_github.py` & `bowtie_json_schema-2024.4.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_hypothesis.py` & `bowtie_json_schema-2024.4.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_integration.py` & `bowtie_json_schema-2024.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_report.py` & `bowtie_json_schema-2024.4.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/test_schemas.py` & `bowtie_json_schema-2024.4.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/.gitignore` & `bowtie_json_schema-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/LICENSE` & `bowtie_json_schema-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/README.rst` & `bowtie_json_schema-2024.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/hatch_build.py` & `bowtie_json_schema-2024.4.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/pyproject.toml` & `bowtie_json_schema-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.9/PKG-INFO` & `bowtie_json_schema-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.3.9
+Version: 2024.4.1
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```


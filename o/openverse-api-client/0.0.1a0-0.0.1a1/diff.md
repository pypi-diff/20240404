# Comparing `tmp/openverse_api_client-0.0.1a0.tar.gz` & `tmp/openverse_api_client-0.0.1a1.tar.gz`

## Comparing `openverse_api_client-0.0.1a0.tar` & `openverse_api_client-0.0.1a1.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/justfile
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/.npmignore
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/package.json
--rw-r--r--   0        0        0    42226 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/pnpm-lock.yaml
--rw-r--r--   0        0        0    12509 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/tsconfig.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/src/.gitignore
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/src/client.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/src/index.ts
--rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/packages/openverse-api-client/src/types.ts
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/.gitignore
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/__about__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/__init__.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/async_client.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/literals.py
--rw-r--r--   0        0        0    16972 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/sync_client.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/auth.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/base.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/media.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/generate/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/generate/base.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/generate/python.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/generate/typescript.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/templates/python/client.py.jinja
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/templates/typescript/types.ts.jinja
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/src/openverse_api_client/templates/typescript/helpers/interface.ts.jinja
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/tests/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/tests/test_async.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/tests/test_sync.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/LICENSE.txt
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/README.md
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.prettierrc.toml
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/justfile
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/.npmignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/LICENSE
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/README.md
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/package.json
+-rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/pnpm-lock.yaml
+-rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tsconfig.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tsconfig.prod.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/vitest.config.mts
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/src/client.ts
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/src/index.ts
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tests/client.test.ts
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tests/mock-thumbnail.bin
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/__about__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/__init__.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/auth.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/meta.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/auth.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/base.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/media.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/__init__.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/base.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/python.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/typescript.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/python/client.py.jinja
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/types.ts.jinja
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/helpers/interface.ts.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/conftest.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/mock-thumbnail.bin
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/test_async.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/test_sync.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/README.rst
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/PKG-INFO
```

### Comparing `openverse_api_client-0.0.1a0/packages/openverse-api-client/tsconfig.json` & `openverse_api_client-0.0.1a1/packages/openverse-api-client/tsconfig.json`

 * *Files 2% similar despite different names*

```diff
@@ -1,110 +1,112 @@
 {
     "compilerOptions": {
-      /* Visit https://aka.ms/tsconfig to read more about this file */
-  
-      /* Projects */
-      // "incremental": true,                              /* Save .tsbuildinfo files to allow for incremental compilation of projects. */
-      // "composite": true,                                /* Enable constraints that allow a TypeScript project to be used with project references. */
-      // "tsBuildInfoFile": "./.tsbuildinfo",              /* Specify the path to .tsbuildinfo incremental compilation file. */
-      // "disableSourceOfProjectReferenceRedirect": true,  /* Disable preferring source files instead of declaration files when referencing composite projects. */
-      // "disableSolutionSearching": true,                 /* Opt a project out of multi-project reference checking when editing. */
-      // "disableReferencedProjectLoad": true,             /* Reduce the number of projects loaded automatically by TypeScript. */
-  
-      /* Language and Environment */
-      "target": "es2016",                                  /* Set the JavaScript language version for emitted JavaScript and include compatible library declarations. */
-      // "lib": [],                                        /* Specify a set of bundled library declaration files that describe the target runtime environment. */
-      // "jsx": "preserve",                                /* Specify what JSX code is generated. */
-      // "experimentalDecorators": true,                   /* Enable experimental support for legacy experimental decorators. */
-      // "emitDecoratorMetadata": true,                    /* Emit design-type metadata for decorated declarations in source files. */
-      // "jsxFactory": "",                                 /* Specify the JSX factory function used when targeting React JSX emit, e.g. 'React.createElement' or 'h'. */
-      // "jsxFragmentFactory": "",                         /* Specify the JSX Fragment reference used for fragments when targeting React JSX emit e.g. 'React.Fragment' or 'Fragment'. */
-      // "jsxImportSource": "",                            /* Specify module specifier used to import the JSX factory functions when using 'jsx: react-jsx*'. */
-      // "reactNamespace": "",                             /* Specify the object invoked for 'createElement'. This only applies when targeting 'react' JSX emit. */
-      // "noLib": true,                                    /* Disable including any library files, including the default lib.d.ts. */
-      // "useDefineForClassFields": true,                  /* Emit ECMAScript-standard-compliant class fields. */
-      // "moduleDetection": "auto",                        /* Control what method is used to detect module-format JS files. */
-  
-      /* Modules */
-      "module": "commonjs",                                /* Specify what module code is generated. */
-      "rootDir": "./src",                                  /* Specify the root folder within your source files. */
-      // "moduleResolution": "node10",                     /* Specify how TypeScript looks up a file from a given module specifier. */
-      // "baseUrl": "./",                                  /* Specify the base directory to resolve non-relative module names. */
-      // "paths": {},                                      /* Specify a set of entries that re-map imports to additional lookup locations. */
-      // "rootDirs": [],                                   /* Allow multiple folders to be treated as one when resolving modules. */
-      // "typeRoots": [],                                  /* Specify multiple folders that act like './node_modules/@types'. */
-      // "types": [],                                      /* Specify type package names to be included without being referenced in a source file. */
-      // "allowUmdGlobalAccess": true,                     /* Allow accessing UMD globals from modules. */
-      // "moduleSuffixes": [],                             /* List of file name suffixes to search when resolving a module. */
-      // "allowImportingTsExtensions": true,               /* Allow imports to include TypeScript file extensions. Requires '--moduleResolution bundler' and either '--noEmit' or '--emitDeclarationOnly' to be set. */
-      // "resolvePackageJsonExports": true,                /* Use the package.json 'exports' field when resolving package imports. */
-      // "resolvePackageJsonImports": true,                /* Use the package.json 'imports' field when resolving imports. */
-      // "customConditions": [],                           /* Conditions to set in addition to the resolver-specific defaults when resolving imports. */
-      // "resolveJsonModule": true,                        /* Enable importing .json files. */
-      // "allowArbitraryExtensions": true,                 /* Enable importing files with any extension, provided a declaration file is present. */
-      // "noResolve": true,                                /* Disallow 'import's, 'require's or '<reference>'s from expanding the number of files TypeScript should add to a project. */
-  
-      /* JavaScript Support */
-      // "allowJs": true,                                  /* Allow JavaScript files to be a part of your program. Use the 'checkJS' option to get errors from these files. */
-      // "checkJs": true,                                  /* Enable error reporting in type-checked JavaScript files. */
-      // "maxNodeModuleJsDepth": 1,                        /* Specify the maximum folder depth used for checking JavaScript files from 'node_modules'. Only applicable with 'allowJs'. */
-  
-      /* Emit */
-      "declaration": true,                              /* Generate .d.ts files from TypeScript and JavaScript files in your project. */
-      "declarationMap": true,                           /* Create sourcemaps for d.ts files. */
-      "emitDeclarationOnly": true,                      /* Only output d.ts files and not JavaScript files. */
-      // "sourceMap": true,                                /* Create source map files for emitted JavaScript files. */
-      // "inlineSourceMap": true,                          /* Include sourcemap files inside the emitted JavaScript. */
-      "outFile": "./dist/index.d.ts",                                  /* Specify a file that bundles all outputs into one JavaScript file. If 'declaration' is true, also designates a file that bundles all .d.ts output. */
-      // "outDir": "./",                                   /* Specify an output folder for all emitted files. */
-      // "removeComments": true,                           /* Disable emitting comments. */
-      // "noEmit": true,                                   /* Disable emitting files from a compilation. */
-      // "importHelpers": true,                            /* Allow importing helper functions from tslib once per project, instead of including them per-file. */
-      // "importsNotUsedAsValues": "remove",               /* Specify emit/checking behavior for imports that are only used for types. */
-      // "downlevelIteration": true,                       /* Emit more compliant, but verbose and less performant JavaScript for iteration. */
-      // "sourceRoot": "",                                 /* Specify the root path for debuggers to find the reference source code. */
-      // "mapRoot": "",                                    /* Specify the location where debugger should locate map files instead of generated locations. */
-      // "inlineSources": true,                            /* Include source code in the sourcemaps inside the emitted JavaScript. */
-      // "emitBOM": true,                                  /* Emit a UTF-8 Byte Order Mark (BOM) in the beginning of output files. */
-      // "newLine": "crlf",                                /* Set the newline character for emitting files. */
-      // "stripInternal": true,                            /* Disable emitting declarations that have '@internal' in their JSDoc comments. */
-      // "noEmitHelpers": true,                            /* Disable generating custom helper functions like '__extends' in compiled output. */
-      // "noEmitOnError": true,                            /* Disable emitting files if any type checking errors are reported. */
-      // "preserveConstEnums": true,                       /* Disable erasing 'const enum' declarations in generated code. */
-      // "declarationDir": "./",                           /* Specify the output directory for generated declaration files. */
-      // "preserveValueImports": true,                     /* Preserve unused imported values in the JavaScript output that would otherwise be removed. */
-  
-      /* Interop Constraints */
-      // "isolatedModules": true,                          /* Ensure that each file can be safely transpiled without relying on other imports. */
-      // "verbatimModuleSyntax": true,                     /* Do not transform or elide any imports or exports not marked as type-only, ensuring they are written in the output file's format based on the 'module' setting. */
-      // "allowSyntheticDefaultImports": true,             /* Allow 'import x from y' when a module doesn't have a default export. */
-      "esModuleInterop": true,                             /* Emit additional JavaScript to ease support for importing CommonJS modules. This enables 'allowSyntheticDefaultImports' for type compatibility. */
-      // "preserveSymlinks": true,                         /* Disable resolving symlinks to their realpath. This correlates to the same flag in node. */
-      "forceConsistentCasingInFileNames": true,            /* Ensure that casing is correct in imports. */
-  
-      /* Type Checking */
-      "strict": true,                                      /* Enable all strict type-checking options. */
-      // "noImplicitAny": true,                            /* Enable error reporting for expressions and declarations with an implied 'any' type. */
-      // "strictNullChecks": true,                         /* When type checking, take into account 'null' and 'undefined'. */
-      // "strictFunctionTypes": true,                      /* When assigning functions, check to ensure parameters and the return values are subtype-compatible. */
-      // "strictBindCallApply": true,                      /* Check that the arguments for 'bind', 'call', and 'apply' methods match the original function. */
-      // "strictPropertyInitialization": true,             /* Check for class properties that are declared but not set in the constructor. */
-      // "noImplicitThis": true,                           /* Enable error reporting when 'this' is given the type 'any'. */
-      // "useUnknownInCatchVariables": true,               /* Default catch clause variables as 'unknown' instead of 'any'. */
-      // "alwaysStrict": true,                             /* Ensure 'use strict' is always emitted. */
-      // "noUnusedLocals": true,                           /* Enable error reporting when local variables aren't read. */
-      // "noUnusedParameters": true,                       /* Raise an error when a function parameter isn't read. */
-      // "exactOptionalPropertyTypes": true,               /* Interpret optional property types as written, rather than adding 'undefined'. */
-      // "noImplicitReturns": true,                        /* Enable error reporting for codepaths that do not explicitly return in a function. */
-      // "noFallthroughCasesInSwitch": true,               /* Enable error reporting for fallthrough cases in switch statements. */
-      // "noUncheckedIndexedAccess": true,                 /* Add 'undefined' to a type when accessed using an index. */
-      // "noImplicitOverride": true,                       /* Ensure overriding members in derived classes are marked with an override modifier. */
-      // "noPropertyAccessFromIndexSignature": true,       /* Enforces using indexed accessors for keys declared using an indexed type. */
-      // "allowUnusedLabels": true,                        /* Disable error reporting for unused labels. */
-      // "allowUnreachableCode": true,                     /* Disable error reporting for unreachable code. */
-  
-      /* Completeness */
-      // "skipDefaultLibCheck": true,                      /* Skip type checking .d.ts files that are included with TypeScript. */
-      "skipLibCheck": true                                 /* Skip type checking all .d.ts files. */
-    }
-  }
-  
+        /* Visit https://aka.ms/tsconfig to read more about this file */
+
+        /* Projects */
+        // "incremental": true,                              /* Save .tsbuildinfo files to allow for incremental compilation of projects. */
+        // "composite": true,                                /* Enable constraints that allow a TypeScript project to be used with project references. */
+        // "tsBuildInfoFile": "./.tsbuildinfo",              /* Specify the path to .tsbuildinfo incremental compilation file. */
+        // "disableSourceOfProjectReferenceRedirect": true,  /* Disable preferring source files instead of declaration files when referencing composite projects. */
+        // "disableSolutionSearching": true,                 /* Opt a project out of multi-project reference checking when editing. */
+        // "disableReferencedProjectLoad": true,             /* Reduce the number of projects loaded automatically by TypeScript. */
+
+        /* Language and Environment */
+        "target": "ESNext" /* Set the JavaScript language version for emitted JavaScript and include compatible library declarations. */,
+        // "lib": [],                                        /* Specify a set of bundled library declaration files that describe the target runtime environment. */
+        // "jsx": "preserve",                                /* Specify what JSX code is generated. */
+        // "experimentalDecorators": true,                   /* Enable experimental support for legacy experimental decorators. */
+        // "emitDecoratorMetadata": true,                    /* Emit design-type metadata for decorated declarations in source files. */
+        // "jsxFactory": "",                                 /* Specify the JSX factory function used when targeting React JSX emit, e.g. 'React.createElement' or 'h'. */
+        // "jsxFragmentFactory": "",                         /* Specify the JSX Fragment reference used for fragments when targeting React JSX emit e.g. 'React.Fragment' or 'Fragment'. */
+        // "jsxImportSource": "",                            /* Specify module specifier used to import the JSX factory functions when using 'jsx: react-jsx*'. */
+        // "reactNamespace": "",                             /* Specify the object invoked for 'createElement'. This only applies when targeting 'react' JSX emit. */
+        // "noLib": true,                                    /* Disable including any library files, including the default lib.d.ts. */
+        // "useDefineForClassFields": true,                  /* Emit ECMAScript-standard-compliant class fields. */
+        // "moduleDetection": "auto",                        /* Control what method is used to detect module-format JS files. */
+
+        /* Modules */
+        "module": "ESNext" /* Specify what module code is generated. */,
+        // "rootDir": "",                                  /* Specify the root folder within your source files. */
+        "moduleResolution": "Bundler" /* Specify how TypeScript looks up a file from a given module specifier. */,
+        // "baseUrl": "./",                                  /* Specify the base directory to resolve non-relative module names. */
+        "paths": {
+            "@openverse/api-client": ["./src"]
+        } /* Specify a set of entries that re-map imports to additional lookup locations. */,
+        // "rootDirs": [],                                   /* Allow multiple folders to be treated as one when resolving modules. */
+        // "typeRoots": [],                                  /* Specify multiple folders that act like './node_modules/@types'. */
+        // "types": [],                                      /* Specify type package names to be included without being referenced in a source file. */
+        // "allowUmdGlobalAccess": true,                     /* Allow accessing UMD globals from modules. */
+        // "moduleSuffixes": [],                             /* List of file name suffixes to search when resolving a module. */
+        // "allowImportingTsExtensions": true,               /* Allow imports to include TypeScript file extensions. Requires '--moduleResolution bundler' and either '--noEmit' or '--emitDeclarationOnly' to be set. */
+        // "resolvePackageJsonExports": true,                /* Use the package.json 'exports' field when resolving package imports. */
+        // "resolvePackageJsonImports": true,                /* Use the package.json 'imports' field when resolving imports. */
+        // "customConditions": [],                           /* Conditions to set in addition to the resolver-specific defaults when resolving imports. */
+        // "resolveJsonModule": true,                        /* Enable importing .json files. */
+        // "allowArbitraryExtensions": true,                 /* Enable importing files with any extension, provided a declaration file is present. */
+        // "noResolve": true,                                /* Disallow 'import's, 'require's or '<reference>'s from expanding the number of files TypeScript should add to a project. */
+
+        /* JavaScript Support */
+        // "allowJs": true,                                  /* Allow JavaScript files to be a part of your program. Use the 'checkJS' option to get errors from these files. */
+        // "checkJs": true,                                  /* Enable error reporting in type-checked JavaScript files. */
+        // "maxNodeModuleJsDepth": 1,                        /* Specify the maximum folder depth used for checking JavaScript files from 'node_modules'. Only applicable with 'allowJs'. */
+
+        /* Emit */
+        "declaration": true /* Generate .d.ts files from TypeScript and JavaScript files in your project. */,
+        "declarationMap": true /* Create sourcemaps for d.ts files. */,
+        "emitDeclarationOnly": true /* Only output d.ts files and not JavaScript files. */,
+        // "sourceMap": true,                                /* Create source map files for emitted JavaScript files. */
+        // "inlineSourceMap": true,                          /* Include sourcemap files inside the emitted JavaScript. */
+        // "outFile": "./dist/index.d.ts" /* Specify a file that bundles all outputs into one JavaScript file. If 'declaration' is true, also designates a file that bundles all .d.ts output. */,
+        "outDir": "./dist" /* Specify an output folder for all emitted files. */,
+        // "removeComments": true,                           /* Disable emitting comments. */
+        // "noEmit": true,                                   /* Disable emitting files from a compilation. */
+        // "importHelpers": true,                            /* Allow importing helper functions from tslib once per project, instead of including them per-file. */
+        // "importsNotUsedAsValues": "remove",               /* Specify emit/checking behavior for imports that are only used for types. */
+        // "downlevelIteration": true,                       /* Emit more compliant, but verbose and less performant JavaScript for iteration. */
+        // "sourceRoot": "",                                 /* Specify the root path for debuggers to find the reference source code. */
+        // "mapRoot": "",                                    /* Specify the location where debugger should locate map files instead of generated locations. */
+        // "inlineSources": true,                            /* Include source code in the sourcemaps inside the emitted JavaScript. */
+        // "emitBOM": true,                                  /* Emit a UTF-8 Byte Order Mark (BOM) in the beginning of output files. */
+        // "newLine": "crlf",                                /* Set the newline character for emitting files. */
+        // "stripInternal": true,                            /* Disable emitting declarations that have '@internal' in their JSDoc comments. */
+        // "noEmitHelpers": true,                            /* Disable generating custom helper functions like '__extends' in compiled output. */
+        // "noEmitOnError": true,                            /* Disable emitting files if any type checking errors are reported. */
+        // "preserveConstEnums": true,                       /* Disable erasing 'const enum' declarations in generated code. */
+        // "declarationDir": "./",                           /* Specify the output directory for generated declaration files. */
+        // "preserveValueImports": true,                     /* Preserve unused imported values in the JavaScript output that would otherwise be removed. */
+
+        /* Interop Constraints */
+        // "isolatedModules": true,                          /* Ensure that each file can be safely transpiled without relying on other imports. */
+        // "verbatimModuleSyntax": true,                     /* Do not transform or elide any imports or exports not marked as type-only, ensuring they are written in the output file's format based on the 'module' setting. */
+        // "allowSyntheticDefaultImports": true,             /* Allow 'import x from y' when a module doesn't have a default export. */
+        "esModuleInterop": true /* Emit additional JavaScript to ease support for importing CommonJS modules. This enables 'allowSyntheticDefaultImports' for type compatibility. */,
+        // "preserveSymlinks": true,                         /* Disable resolving symlinks to their realpath. This correlates to the same flag in node. */
+        "forceConsistentCasingInFileNames": true /* Ensure that casing is correct in imports. */,
+
+        /* Type Checking */
+        "strict": true /* Enable all strict type-checking options. */,
+        // "noImplicitAny": true,                            /* Enable error reporting for expressions and declarations with an implied 'any' type. */
+        // "strictNullChecks": true,                         /* When type checking, take into account 'null' and 'undefined'. */
+        // "strictFunctionTypes": true,                      /* When assigning functions, check to ensure parameters and the return values are subtype-compatible. */
+        // "strictBindCallApply": true,                      /* Check that the arguments for 'bind', 'call', and 'apply' methods match the original function. */
+        // "strictPropertyInitialization": true,             /* Check for class properties that are declared but not set in the constructor. */
+        // "noImplicitThis": true,                           /* Enable error reporting when 'this' is given the type 'any'. */
+        // "useUnknownInCatchVariables": true,               /* Default catch clause variables as 'unknown' instead of 'any'. */
+        // "alwaysStrict": true,                             /* Ensure 'use strict' is always emitted. */
+        // "noUnusedLocals": true,                           /* Enable error reporting when local variables aren't read. */
+        // "noUnusedParameters": true,                       /* Raise an error when a function parameter isn't read. */
+        // "exactOptionalPropertyTypes": true,               /* Interpret optional property types as written, rather than adding 'undefined'. */
+        // "noImplicitReturns": true,                        /* Enable error reporting for codepaths that do not explicitly return in a function. */
+        // "noFallthroughCasesInSwitch": true,               /* Enable error reporting for fallthrough cases in switch statements. */
+        // "noUncheckedIndexedAccess": true,                 /* Add 'undefined' to a type when accessed using an index. */
+        // "noImplicitOverride": true,                       /* Ensure overriding members in derived classes are marked with an override modifier. */
+        // "noPropertyAccessFromIndexSignature": true,       /* Enforces using indexed accessors for keys declared using an indexed type. */
+        // "allowUnusedLabels": true,                        /* Disable error reporting for unused labels. */
+        // "allowUnreachableCode": true,                     /* Disable error reporting for unreachable code. */
+
+        /* Completeness */
+        // "skipDefaultLibCheck": true,                      /* Skip type checking .d.ts files that are included with TypeScript. */
+        "skipLibCheck": true /* Skip type checking all .d.ts files. */
+    },
+    "exclude": ["./dist/**"]
+}
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/auth.py` & `openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from typing import TypedDict, Literal, NotRequired
+from typing_extensions import TypedDict, Literal
 
 from openverse_api_client.endpoints.base import OpenverseAPIEndpoint
 
 
 class POST_v1_auth_tokens_register(OpenverseAPIEndpoint):
     method = "POST"
     endpoint = "v1/auth_tokens/register/"
 
     class params(TypedDict, total=True):
         name: str
         description: str
         email: str
 
-
     class response(TypedDict, total=True):
         name: str
         client_id: str
         client_secret: str
 
 
 class POST_v1_auth_tokens_token(OpenverseAPIEndpoint):
     method = "POST"
     endpoint = "v1/auth_tokens/token/"
     content_type = "application/x-www-form-urlencoded"
 
     class params(TypedDict, total=True):
-        grant_type: Literal["client_credentials"] = "client_credentials"
+        grant_type: Literal["client_credentials"]
         client_id: str
         client_secret: str
 
     class response(TypedDict, total=True):
         access_token: str
         scope: str
         expires_in: int
@@ -37,14 +36,15 @@
 
 
 class GET_v1_rate_limit(OpenverseAPIEndpoint):
     method = "GET"
     endpoint = "v1/rate_limit/"
 
     # Based entirely on bearer token
-    params = None
+    class params(TypedDict):
+        pass
 
     class response(TypedDict, total=True):
         requests_this_minute: int | None
         requests_today: int | None
         rate_limit_model: Literal["standard", "enhanced"]
         verified: bool
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/endpoints/media.py` & `openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/media.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-from typing import TypedDict, Literal, Required, NotRequired
+from typing_extensions import TypedDict, Required, Literal, Type, TypeAlias
 from decimal import Decimal
 
 from openverse_api_client.endpoints.base import OpenverseAPIEndpoint
-from openverse_api_client import literals
+
+
+_MediaTypePlural = Literal["images", "audio"]
+_MediaTypeSingular = Literal["image", "audio"]
 
 
 class SourceStats(TypedDict, total=True):
     source_name: str
     display_name: str
     source_url: str
     media_count: int
+    logo_url: str
 
-def _GET_v1___stats(media_type: literals.MediaTypePlural):
 
+def _GET_v1___stats(media_type: _MediaTypePlural):
     return type(
         f"GET_v1_{media_type}_stats",
         (OpenverseAPIEndpoint,),
         {
             "method": "GET",
             "endpoint": f"v1/{media_type}/stats/",
             "params": None,
-            "response": list[SourceStats]
-        }
+            "response": list[SourceStats],
+        },
     )
 
+
 GET_v1_images_stats = _GET_v1___stats("images")
 GET_v1_audio_stats = _GET_v1___stats("audio")
 
 
 class _BaseSearchParams(TypedDict, total=False):
     page: int
     page_size: int
@@ -52,34 +57,30 @@
 
 class _ImageSearchParams(TypedDict, total=False):
     category: str | list[str]
     aspect_ratio: str | list[str]
     size: list[str]
 
 
-class _ImageByQuerySearchParams(_ImageSearchParams, _ByQuerySearchParams):
-    ...
+class _ImageByQuerySearchParams(_ImageSearchParams, _ByQuerySearchParams): ...
 
 
-class _ImageByFieldSearchParams(_ImageSearchParams, _ByFieldSearchParams):
-    ...
+class _ImageByFieldSearchParams(_ImageSearchParams, _ByFieldSearchParams): ...
 
 
 class _AudioSearchParams(TypedDict, total=False):
     category: str | list[str]
     length: str | list[str]
     peaks: bool
 
 
-class _AudioByQuerySearchParams(_AudioSearchParams, _ByQuerySearchParams):
-    ...
+class _AudioByQuerySearchParams(_AudioSearchParams, _ByQuerySearchParams): ...
 
 
-class _AudioByFieldSearchParams(_AudioSearchParams, _ByFieldSearchParams):
-    ...
+class _AudioByFieldSearchParams(_AudioSearchParams, _ByFieldSearchParams): ...
 
 
 class Tag(TypedDict, total=False):
     name: Required[str]
     accuracy: Decimal | None
 
 
@@ -121,15 +122,15 @@
 
 
 class GET_v1_images(OpenverseAPIEndpoint):
     method = "GET"
     endpoint = "v1/images/"
 
     # Note: need to use overloads to type the client method kwargs
-    params = _ImageByQuerySearchParams | _ImageByFieldSearchParams
+    params = Type[_ImageByQuerySearchParams] | Type[_ImageByFieldSearchParams]
 
     class response(_SearchResponse):
         results: list[ImageDetail]
 
 
 class AudioSet(TypedDict, total=True):
     title: str | None
@@ -152,88 +153,112 @@
     genres: list[str] | None
 
 
 class GET_v1_audio(OpenverseAPIEndpoint):
     method = "GET"
     endpoint = "v1/audio/"
 
-    params = _AudioByQuerySearchParams | _AudioByFieldSearchParams
+    params = Type[_AudioByQuerySearchParams] | Type[_AudioByFieldSearchParams]
 
     class response(_SearchResponse):
         results: list[AudioDetail]
 
 
-def _GET_v1___related(media_type: literals.MediaTypePlural):
-    class params(TypedDict, total=True):
+class GET_v1_single_image(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/images/:identifier/"
+    path_params = ("identifier",)
+
+    class params(TypedDict, total=False):
         identifier: str
 
-    response = GET_v1_audio.response if media_type == "audio" else GET_v1_images.response
+    response = Type[ImageDetail]
 
-    return type(
-        f"GET_v1_{media_type}_related",
-        (OpenverseAPIEndpoint,),
-        {
-            "method": "GET",
-            "endpoint": f"v1/{media_type}/:identifier/related",
-            "path_params": ("identifier",),
-            "params": params,
-            "response": response,
-        }
-    )
 
+class GET_v1_single_audio(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/audio/:identifier/"
+    path_params = ("identifier",)
+
+    class params(TypedDict, total=False):
+        identifier: str
 
-GET_v1_images_related = _GET_v1___related("images")
-GET_v1_audio_related = _GET_v1___related("audio")
+    response = Type[AudioDetail]
 
 
-def _GET_v1___thumbnail(media_type: literals.MediaTypePlural):
+class GET_v1_images_related(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/images/:identifier/related/"
+    path_params = ("identifier",)
+
     class params(TypedDict, total=False):
-        identifier: Required[str]
+        identifier: str
+
+    response = Type[ImageDetail]
+
+
+class GET_v1_audio_related(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/audio/:identifier/related/"
+    path_params = ("identifier",)
+
+    class params(TypedDict, total=False):
+        identifier: str
+
+    response = Type[AudioDetail]
+
+
+class GET_v1_images_thumbnail(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/images/:identifier/thumb/"
+    path_params = ("identifier",)
+
+    class params(TypedDict, total=False):
+        identifier: str
         full_size: bool
         compressed: bool
 
+    response: TypeAlias = bytes
 
-    return type(
-        f"GET_v1_{media_type}_thumbnail",
-        (OpenverseAPIEndpoint,),
-        {
-            "method": "GET",
-            "endpoint": f"v1/{media_type}/:identifier/thumb/",
-            "path_params": ("identifier",),
-            "params": params,
-            "response": bytes,
-        }
-    )
 
+class GET_v1_audio_thumbnail(OpenverseAPIEndpoint):
+    method = "GET"
+    endpoint = "v1/audio/:identifier/thumb/"
+    path_params = ("identifier",)
 
-GET_v1_images_thumbnail = _GET_v1___thumbnail("images")
-GET_v1_audio_thumbnail = _GET_v1___thumbnail("audio")
+    class params(TypedDict, total=False):
+        identifier: str
+        full_size: bool
+        compressed: bool
+
+    # class response(bytes):
+    # pass
+    response: TypeAlias = bytes
 
 
 class GET_v1_audio_waveform(OpenverseAPIEndpoint):
     method = "GET"
     endpoint = "v1/audio/:identifier/waveform/"
-
     path_params = ("identifier",)
 
-    class params(TypedDict, total=True):
+    class params(TypedDict, total=False):
         identifier: str
-    
+
     class response(TypedDict, total=True):
         len: int
         points: list[int]
 
 
 class GET_v1_images_oembed(OpenverseAPIEndpoint):
     method = "GET"
     endpoint = "v1/images/oembed"
 
     class params(TypedDict, total=True):
         url: str
-    
+
     class response(TypedDict, total=True):
         version: str
         type: str
         width: int
         height: int
         title: str | None
         author_name: str | None
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/generate/python.py` & `openverse_api_client-0.0.1a1/src/openverse_api_client/generate/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 import inspect
-from typing import Union, TypedDict, get_args
+from typing import TypedDict, get_args
 
 from openverse_api_client import endpoints
-from openverse_api_client.generate.base import template_env
+from openverse_api_client.generate.base import template_env, is_bytes
+from openverse_api_client.meta import empty
 
 
 client_template = template_env.get_template("python/client.py.jinja")
 
 
 def type_to_string(t) -> str:
     if isinstance(t, str):
         return f"'{str(t)}'"
     elif not hasattr(t, "__name__"):
         return str(t)
 
     if t.__name__ == "Literal":
-        literals = ", ".join(
-            [
-                type_to_string(a)
-                for a in get_args(t)
-            ]
-        )
-        return f'Literal[{literals}]'
-    elif t.__name__ == "Required":
+        literals = ", ".join([type_to_string(a) for a in get_args(t)])
+        return f"Literal[{literals}]"
+    elif t.__name__ in ["Required", "Type"]:
         return type_to_string(get_args(t)[0])
     return t.__name__
 
 
 PythonFiles = TypedDict("PythonFiles", {"async_client.py": str, "sync_client.py": str})
 
 
-_empty = object()
-
-
 def generate_python() -> PythonFiles:
     methods = []
 
     for endpoint in endpoints.OpenverseAPIEndpoint.__subclasses__():
         signatures = []
         param_definitions = getattr(endpoint.params, "__args__", [endpoint.params])
         for param_def in param_definitions:
             parameters = []
             if param_def:
+                if getattr(param_def, "__name__", None) == "Type":
+                    param_def = get_args(param_def)[0]
+
                 for name, annotation in inspect.get_annotations(param_def).items():
-                    required = name in param_def.__required_keys__
+                    required = (
+                        name in param_def.__required_keys__
+                        or name in endpoint.path_params
+                    )
                     param = {
                         "name": name,
                         "type": type_to_string(annotation),
                         "required": required,
                     }
 
-                    default = getattr(param_def, name, _empty)
-                    if default != _empty:
+                    default = getattr(param_def, name, empty)
+                    if default != empty:
                         param["default"] = type_to_string(default)
 
                     parameters.append(param)
 
-            parameters.sort(key=lambda x: 1 if "default" in x or not x["required"] else 0)
+            parameters.sort(
+                key=lambda x: 1 if "default" in x or not x["required"] else 0
+            )
 
             signature = dict(
-                parameters=parameters,
-                return_annotation=endpoint.response.__name__
+                parameters=parameters, return_annotation=endpoint.response.__name__
             )
             signatures.append(signature)
 
         methods.append(
             {
                 "signatures": signatures,
                 "overloaded": len(signatures) > 1,
                 "endpoint": endpoint,
-                "json_response": endpoint.response is not bytes,
+                "json_response": not is_bytes(endpoint.response),
             }
         )
-    
+
     async_client = client_template.render(
         **{
             "methods": methods,
             "await": "await ",
             "a": "a",
             "def": "async def",
             "Async": "Async",
@@ -89,11 +89,13 @@
             "await": "",
             "a": "",
             "def": "def",
             "Async": "",
         }
     )
 
-    return PythonFiles(**{
-        "async_client.py": async_client,
-        "sync_client.py": sync_client,
-    })
+    return PythonFiles(
+        **{
+            "async_client.py": async_client,
+            "sync_client.py": sync_client,
+        }
+    )
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/generate/typescript.py` & `openverse_api_client-0.0.1a1/src/openverse_api_client/generate/typescript.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import inspect
-from typing import TypedDict, Any, GenericAlias, _TypedDictMeta, get_origin, get_args
+from typing_extensions import Set, TypedDict, get_args, _TypedDictMeta, is_typeddict  # type: ignore[attr-defined]
 from types import UnionType, NoneType
 from decimal import Decimal
 from dataclasses import dataclass, asdict
 
 
 from openverse_api_client import endpoints
-from openverse_api_client.generate.base import template_env
+from openverse_api_client.generate.base import template_env, is_bytes
 
 
-TypeScriptFiles = TypedDict("TypeScriptFiles", {
-    "types.ts": str,
-})
+TypeScriptFiles = TypedDict(
+    "TypeScriptFiles",
+    {
+        "types.ts": str,
+    },
+)
 
 
 @dataclass(unsafe_hash=True)
 class TSProperty:
     name: str
     required: bool
     type: str
@@ -29,39 +32,43 @@
     def __hash__(self) -> int:
         return f"{self.interface_name}; {','.join((str(p) for p in self.properties))}".__hash__()
 
 
 interface_template = template_env.get_template("typescript/helpers/interface.ts.jinja")
 types_template = template_env.get_template("typescript/types.ts.jinja")
 
-def map_typed_dict_to_ts_object_meta(d: _TypedDictMeta) -> TSObjectMeta:
+
+def map_typed_dict_to_ts_object_meta(
+    endpoint: endpoints.OpenverseAPIEndpoint, d: _TypedDictMeta
+) -> TSObjectMeta:
     """
     Map a Python TypedDict property.
     """
 
     properties = []
     for p_name, p_type in inspect.get_annotations(d).items():
         properties.append(
             TSProperty(
                 name=p_name,
-                required=p_name in d.__required_keys__,
-                type=map_python_type(p_type),
+                required=p_name in d.__required_keys__
+                or p_name in endpoint.path_params,
+                type=map_python_type(endpoint, p_type),
             )
         )
 
     return TSObjectMeta(
         interface_name=d.__name__,
         properties=properties,
     )
 
 
-interfaces = set()
+interfaces: Set[TSObjectMeta] = set()
 
 
-def map_python_type(t: type | GenericAlias) -> str:
+def map_python_type(endpoint: endpoints.OpenverseAPIEndpoint, t: type) -> str:
     """
     Map a Python type to the equivalent TypeScript type.
     """
 
     if t is None or t == NoneType:
         return "null"
     elif t is str:
@@ -69,43 +76,47 @@
     elif t is bool:
         return "boolean"
     elif t is bytes:
         return "ReadableStream"
     elif t is int or t is Decimal:
         return "number"
     elif isinstance(t, UnionType):
-        return " | ".join((map_python_type(a) for a in get_args(t)))
-    elif isinstance(t, _TypedDictMeta):
+        return " | ".join((map_python_type(endpoint, a) for a in get_args(t)))
+    elif is_typeddict(t):
         # Add to ambient interfaces
-        interfaces.add(map_typed_dict_to_ts_object_meta(t))
+        interfaces.add(map_typed_dict_to_ts_object_meta(endpoint, t))
         return t.__name__
     elif hasattr(t, "__name__"):
         match t.__name__:
+            case "Type":
+                return map_python_type(endpoint, get_args(t)[0])
             case "Literal":
                 # Literal accepts multiple arguments, rather than
                 # a single union argument. In TS, that translates
                 # to a union of "literals", e.g., `type Category = 'photo' | 'illustration'`
                 args = []
                 for arg in get_args(t):
                     if isinstance(arg, str):
                         args.append(f"'{arg}'")
                     else:
                         args.append(arg)
                 return " | ".join(args)
             case "Required":
-                return map_python_type(get_args(t)[0])
+                return map_python_type(endpoint, get_args(t)[0])
             case "list" | "Iterable" | "Sequence":
                 # Use `Array` instead of `[]` shorthand to avoid
                 # complications with a Union as the argument
-                return f"Array<{map_python_type(get_args(t)[0])}>"
+                return f"Array<{map_python_type(endpoint, get_args(t)[0])}>"
             case "tuple":
-                args = ", ".join(())
-                return f"[{map_python_type}]"
+                tuple_args = ", ".join(
+                    [map_python_type(endpoint, a) for a in get_args(t)]
+                )
+                return f"[{tuple_args}]"
             case "dict" | "Mapping":
-                args = [map_python_type(a) for a in get_args(t)]
+                args = [map_python_type(endpoint, a) for a in get_args(t)]
                 if not args:
                     return "Record<string, any>"
                 if len(args) == 1:
                     args = [args[0], args[0]]
                 return f"Record<{', '.join(args)}>"
 
     raise ValueError(f"Unsupported type {t}")
@@ -117,52 +128,51 @@
     requests = []
 
     for endpoint in endpoints.OpenverseAPIEndpoint.__subclasses__():
         request = {
             "name": f"{endpoint.method} {endpoint.endpoint}",
             "content_type": endpoint.content_type,
             "path_params": endpoint.path_params,
-            "json_response": isinstance(endpoint.response, _TypedDictMeta),
+            "json_response": not is_bytes(endpoint.response),
         }
         if not endpoint.params:
             request["params"] = None
         elif isinstance(endpoint.params, UnionType):
             for arg in get_args(endpoint.params):
-                obj_meta = map_typed_dict_to_ts_object_meta(arg)
+                obj_meta = map_typed_dict_to_ts_object_meta(endpoint, arg)
                 interfaces.add(obj_meta)
-            request["params"] = " | ".join((a.__name__ for a in get_args(endpoint.params)))
+            request["params"] = " | ".join(
+                (a.__name__ for a in get_args(endpoint.params))
+            )
         else:
-            obj_meta = map_typed_dict_to_ts_object_meta(endpoint.params)
+            obj_meta = map_typed_dict_to_ts_object_meta(endpoint, endpoint.params)
             if obj_meta.interface_name != "params":
                 interfaces.add(obj_meta)
                 request["params"] = obj_meta.interface_name
             else:
                 request["params"] = obj_meta.properties
 
         if isinstance(endpoint.response, _TypedDictMeta):
-            obj_meta = map_typed_dict_to_ts_object_meta(endpoint.response)
+            obj_meta = map_typed_dict_to_ts_object_meta(endpoint, endpoint.response)
             if obj_meta.interface_name != "response":
                 interfaces.add(obj_meta)
                 request["response"] = obj_meta.interface_name
             else:
                 request["response"] = obj_meta.properties
         else:
-            request["response"] = map_python_type(endpoint.response)
+            request["response"] = map_python_type(endpoint, endpoint.response)
 
         requests.append(request)
-    
+
     rendered_interfaces = [
-        interface_template.render(**asdict(interface))
-        for interface in interfaces
+        interface_template.render(**asdict(interface)) for interface in interfaces
     ]
     context = {
         "interfaces": rendered_interfaces,
         "requests": requests,
     }
 
     return types_template.render(**context)
 
 
 def generate_typescript() -> TypeScriptFiles:
-    return TypeScriptFiles(**{
-        "types.ts": render_types()
-    })
+    return TypeScriptFiles(**{"types.ts": render_types()})
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/templates/python/client.py.jinja` & `openverse_api_client-0.0.1a1/src/openverse_api_client/templates/python/client.py.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,152 +1,136 @@
 """
 This file is generated by `openverse_api_client`, do not edit it directly.
 """
 
 from datetime import datetime, timedelta, UTC
-from typing import Any, cast, Self, Literal, overload
+from typing_extensions import Dict, Any, cast, Self, Literal, overload
 import httpx
-
+{%- if Async %}
+import asyncio
+{%- endif %}
 
 from openverse_api_client import endpoints
+from openverse_api_client.auth import OpenverseAuth
+from openverse_api_client.meta import Empty, empty, OpenverseAPIResponse, OpenverseAPIRequest
 
 
 EXPIRY_THRESHOLD = 30
 
 
-_empty = object()
-
-
 class {{ Async }}OpenverseClient:
-    api_token: endpoints.POST_v1_auth_tokens_token.response | None = None 
-    token_expiry: datetime | None = None
-    credentials: endpoints.POST_v1_auth_tokens_token.params | None = None
-
     base_url: str = "https://api.openverse.engineering/"
-
+    auth: OpenverseAuth | None = None
     client: httpx.{{ Async }}Client
+
     _is_shared_client: bool
 
     def __init__(
         self,
         base_url: str | None = None,
         client_id: str | None = None,
         client_secret: str | None = None,
         httpx_client: httpx.{{ Async }}Client | None = None,
     ):
         self.base_url = base_url if base_url else self.base_url
         if self.base_url[-1] != "/":
             self.base_url += "/"
-        
+
         if client_id or client_secret:
             assert client_id and client_secret, "`client_id` and `client_secret` are both required when either is defined"
-            
-            self.credentials = endpoints.POST_v1_auth_tokens_token.params(
-                grant_type="client_credentials",
+
+            self.auth = OpenverseAuth(
+                client=self,
                 client_id=client_id,
                 client_secret=client_secret,
             )
-        
+
         if httpx_client is None:
             self.client = httpx.{{ Async }}Client()
             self._is_shared_client = False
         else:
             self.client = httpx_client
             self._is_shared_client = True
-    
+
     {{ def }} __{{ a }}enter__(self) -> Self:
         return self
 
     {{ def }} __{{ a }}exit__(self, exc_type=None, exc_value=None, traceback=None) -> None:
         {{ await }}self.client.__{{ a }}exit__(exc_type, exc_value, traceback)
 
     {{ def }} close(self):
         {{ await }}self.client.{{ a }}close()
 
     {{ def }} _base_request(
         self,
+        *,
         method: str,
         path: str,
-        params: dict,
-        headers: httpx.Headers,
+        **kwargs,
     ) -> httpx.Response:
         return {{ await }}self.client.request(
             method=method,
             url=f"{self.base_url}{path}",
-            params=params,
-            headers=headers,
+            **kwargs,
         )
-    
+
     {{ def }} _request(
         self,
+        *,
         method: str,
         path: str,
-        params: dict,
-        headers: httpx.Headers,
+        **kwargs,
     ) -> httpx.Response:
+        kwargs.setdefault("auth", self.auth)
         return {{ await }}self._base_request(
             method=method,
             path=path,
-            params=params,
-            headers=headers.update({{ await }}self._get_auth_headers())
+            **kwargs,
         )
-
-    {{ def }} _get_auth_headers(self) -> dict:
-        if self.credentials is None:
-            return {}
-        
-        if self.api_token is None or self.token_expiry < datetime.now():
-            endpoint = endpoints.POST_v1_auth_tokens_token
-            token_response = {{ await }}self._base_request(
-                method=endpoint.method,
-                path=endpoint.endpoint,
-                params=self.credentials,
-            )
-
-            {{ await }}token_response.{{ a }}read()
-            self.api_token = cast(endpoint.response, token_response.json())
-            self.token_expiry = datetime.now(UTC) + timedelta(seconds=self.api_token["expires_in"] - EXPIRY_THRESHOLD)
-        
-        return {"Authorization": f"Bearer {self.api_token['access_token']}"}
-    
     {% for method in methods -%}
     {% for signature in method.signatures -%}
     {% if method.overloaded %}
     @overload
     {%- endif %}
     {{ def }} {{ method.endpoint.__name__ }}(
         self,
         {% for param in signature.parameters -%}
-        {{ param.name }}: {{ param.type }}
+        {{ param.name }}: {{ param.type }}{% if not param.required %} | Empty{% endif %}
         {%- if param.default is defined %} = {{ param.default }}
-        {%- elif not param.required %} = _empty
+        {%- elif not param.required %} = empty
         {%- endif %},
         {% endfor -%}
         headers: dict | httpx.Headers | None = None
-    ) -> endpoints.{{ method.endpoint.__name__ }}.response:
+    ) -> OpenverseAPIResponse[endpoints.{{ method.endpoint.__name__ }}.response]:
         {%- if method.overloaded %}
         ...{% endif -%}
     {% endfor -%}
         {%- if method.overloaded %}
     {{ def }} {{ method.endpoint.__name__ }}(self, **kwargs):
         headers = kwargs.pop("headers", None)
-        params = kwargs
+        params = cast(endpoints.{{ method.endpoint.__name__ }}.params, kwargs)
         {%- else %}
-        params = {
-            {%- for param in (method.signatures | first).parameters %}
-            "{{ param.name }}": {{ param.name }},
-            {%- endfor %}
-        }
+        params = cast(
+            endpoints.{{ method.endpoint.__name__ }}.params,
+            {
+                {%- for param in (method.signatures | first).parameters %}
+                "{{ param.name }}": {{ param.name }},
+                {%- endfor %}
+            }
+        )
         {%- endif %}
 
-        params = {
-            k: v
-            for k, v in params.items()
-            if v != _empty
-        }
+        params = cast(
+            endpoints.{{ method.endpoint.__name__ }}.params,
+            {
+                k: v
+                for k, v in params.items()
+                if v != empty
+            }
+        )
 
         path = "{{ method.endpoint.endpoint }}"
 
         {%- for path_param in method.endpoint.path_params %}
         path = path.replace(":{{ path_param }}", params["{{ path_param }}"])
         del params["{{ path_param }}"]
         {%- endfor %}
@@ -163,9 +147,17 @@
 
         {{ await }}response.{{ a }}read()
         {% if method.json_response -%}
         content = response.json()
         {% else -%}
         content = response.content
         {% endif -%}
-        return cast(endpoints.{{ method.endpoint.__name__ }}.response, content)
+        return OpenverseAPIResponse(
+            body=content,
+            headers=response.headers,
+            status_code=response.status_code,
+            request=OpenverseAPIRequest(
+                headers=headers,
+                params=params,
+            )
+        )
     {% endfor -%}
```

### Comparing `openverse_api_client-0.0.1a0/src/openverse_api_client/templates/typescript/types.ts.jinja` & `openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/types.ts.jinja`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a0/README.md` & `openverse_api_client-0.0.1a1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,81 @@
 # openverse-api-client
 
 Fully typed Openverse API clients for Python and JavaScript.
 
+[![Repository](https://img.shields.io/badge/sr.ht-~sara%2Fopenverse--api--client-%23c52b9b?logo=sourcehut)](https://sr.ht/~sara/openverse-api-client)
 [![PyPI - Version](https://img.shields.io/pypi/v/openverse-api-client.svg)](https://pypi.org/project/openverse-api-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openverse-api-client.svg)](https://pypi.org/project/openverse-api-client)
+[![NPM Version](https://img.shields.io/npm/v/%40openverse%2Fapi-client)](https://www.npmjs.com/package/@openverse/api-client)
 
------
+---
 
-## Installation
+## Client libraries
 
-**Python**
-
-```console
-pip install openverse-api-client
-```
-
-**JavaScript**
-
-```console
-npm install @openverse/api-client
-```
+-   Python: https://pypi.org/project/openverse-api-client
+-   JavaScript: https://www.npmjs.com/package/@openverse/api-client
 
 ## Development
 
 **Dependencies**:
-- `hatch`
-- `pnpm`
-- `just`
 
-This project generates Python and TypeScript clients for the Openverse API, based on endpoint definitions written in Python, and Jinja2 templates for Python and TypeScript files. A full build of both clients requires the following steps:
+-   `hatch`
+-   `pnpm`
+-   `just`
+
+This project generates Python and TypeScript clients for the Openverse API,
+based on endpoint definitions written in Python, and Jinja2 templates for Python
+and TypeScript files. A full build of both clients requires the following steps:
 
 1. Generating the client code: `hatch run generate`
-2. Building the npm package (including TypeScript definitions): `just pnpm build`
+2. Building the npm package (including TypeScript definitions):
+   `just pnpm build`
+    - Run `just pnpm install` if this is the first run
 3. Building the Python package: `hatch build`
 
-The `just build` recipe encapsulates these tasks into a single command. Each task can run on its own for debugging different parts of the client code generation or build process.
+The `just build` recipe encapsulates these tasks into a single command. Each
+task can run on its own for debugging different parts of the client code
+generation or build process.
+
+In most cases, you will need to run at least `hatch run generate` for
+development tools to work, because otherwise critical files will be missing that
+other runtime code depends on.
+
+The Python clients live in the same package as the client generation code, which
+allows them to reuse the endpoint definitions for Python type hints without
+introducing an intermediary package. The Jinja2 dependency is optional, and only
+installed when the `generator` feature is installed (i.e.,
+`pip install openverse-api-client[generator]`).
+
+The CLI (`generate-openverse-api-client` or `hatch run generate`) accepts
+arguments to control which languages are generated. Run `hatch run generate -h`
+to view the CLI documentation.
+
+Tests for both the Python and JavaScript clients should be run using `just`
+recipes, which manage cleaning and regeneration of the clients on each run. For
+Python:
+
+```shell
+just pytest
+```
+
+For JavaScript/TypeScript:
+
+```shell
+just tstest
+```
+
+### Contributing
 
-In most cases, you will need to run at least `hatch run generate` for development tools to work, because otherwise critical files will be missing that other runtime code depends on.
+Contributions are welcome using patchsets. You can submit these either via
+Sourcehut's UI, or `git send-email`. Please refer to Sourcehut's documentation
+and tutorial for this process:
+https://man.sr.ht/git.sr.ht/#sending-patches-upstream.
 
-The Python clients live in the same package as the client generation code, which allows them to reuse the endpoint definitions for Python type hints without introducing an intermediary package. The Jinja2 dependency is optional, and only installed when the `generator` feature is installed (i.e., `pip install openverse-api-client[generator]`).
+Please send patches to
+[`~sara/openverse-api-client-devel@lists.sr.ht`](mailto:~sara/openverse-api-client-devel@lists.sr.ht).
 
 ## License
 
-`openverse-api-client` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`openverse-api-client` is distributed under the terms of the
+[GNU Lesser General Public License v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html)
+license.
```

### Comparing `openverse_api_client-0.0.1a0/pyproject.toml` & `openverse_api_client-0.0.1a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,81 +2,86 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openverse-api-client"
 dynamic = ["version"]
 description = 'Python client for the Openverse API'
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.8"
-license = "MIT"
 keywords = []
 authors = [
-  { name = "sarayourfriend", email = "24264157+sarayourfriend@users.noreply.github.com" },
+  { name = "sarayourfriend", email = "git@sarayourfriend.pictures" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dependencies = [
   "httpx",
 ]
 
 [project.optional-dependencies]
 generator = [
   "Jinja2",
 ]
 
+[project.license]
+file = "LICENSE"
+
 [project.urls]
+Homepage = "https://sr.ht/~sara/openverse-api-client/#openverse-api-client"
 Documentation = "https://git.sr.ht/~sara/openverse-api-client#readme"
-Issues = "https://git.sr.ht/~sara/openverse-api-client/issues"
+Issues = "https://todo.sr.ht/~sara/openverse-api-client"
 Source = "https://git.sr.ht/~sara/openverse-api-client"
 
 [project.scripts]
-generate-openverse-api-client = "openverse_api_client.generate:generate"
+generate-openverse-api-client = "openverse_api_client.generate:generate_cli"
 
 [tool.hatch.version]
 path = "src/openverse_api_client/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
+  "mypy>=1.0.0",
+  "typing_extensions",
   "pytest",
   "pytest-asyncio",
+  "pytest-pook",
+  "pook",
+  "pre-commit",
 ]
 features = ["generator"]
 [tool.hatch.envs.default.scripts]
-generate = "generate-openverse-api-client"
+generate = "generate-openverse-api-client {args}"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+lint-install = "pre-commit install"
+lint = "pre-commit run --all-files"
+types = "mypy --install-types --non-interactive {args:src/openverse_api_client tests}"
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
-
-[tool.hatch.envs.types]
-dependencies = [
-  "mypy>=1.0.0",
-]
-[tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/openverse_api_client tests}"
+python = ["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3.11"]
 
 [tool.coverage.run]
 source_pkgs = ["openverse_api_client", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/openverse_api_client/__about__.py",
```


# Next.js 15 Build Error: Missing Export

This repository demonstrates a seemingly inexplicable build error in Next.js 15 where a default export is correctly defined, but the build process still reports a missing export.  This issue has been observed in projects using various configurations and appears to be intermittent in nature.

## Bug Description

The `pages/index.js` file contains a simple component with a default export. However, running `next build` results in a build failure indicating that an export is missing.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install`.
3. Run `next build`.

## Expected Behavior

The build process should complete successfully without reporting any missing exports.

## Actual Behavior

The build process fails with an error stating that an export is missing in `pages/index.js` despite the obvious presence of a default export.

## Potential Causes

* **Caching Issues:**  Next.js build cache might be corrupt.
* **Plugin Conflicts:** A conflicting plugin or configuration setting could be interfering with the build process.
* **Version Inconsistencies:** Specific versions of Next.js or related dependencies might contribute to this problem.
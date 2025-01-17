The path to your scan results when running an [Ingestion scan](/docs/security-testing-orchestration/use-sto/orchestrate-and-ingest/ingest-scan-results-into-an-sto-pipeline), for example `/shared/scan_results/myscan.latest.sarif`.  

- The data file must be in a [supported format](/docs/security-testing-orchestration/sto-techref-category/security-step-settings-reference#supported-ingestion-formats) for the scanner.

- The data file must be accessible to the scan step. It's good practice to save your results files to a [shared path](/docs/continuous-integration/get-started/key-concepts#stages) in your stage. To add the path, go to **Overview** > **Shared Paths** in the visual editor. You can also add it the YAML stage definition like this:  
  
  ```yaml
      - stage:
        spec:
          sharedPaths:
            - /shared/scan_results
  ``` 
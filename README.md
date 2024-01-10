# UiPath-Analyze
Runs workflow analysis with stopOnRuleViolation enabled for all UiPath projects in a GitHub repository.

Example usage:

      # Action for packing UiPath projects in a repository
      - name: UiPath Analyze
        uses: Mikael-RnD/UiPath-Analyze@main
        with:
          # All inputs are required
          orchestratorUrl: # Link to UiPath Orchestrator instance
          orchestratorTenant: # Name of tenant where packages are deployed
          orchestratorFolder: # Orchestrator Folder path where packages are deployed
          orchestratorApplicationId: # Applicaiton Id for External Application in Orchestrator
          orchestratorApplicationSecret: # Application Secret for External Application in Orchestrator
          orchestratorApplicationScope: # Scope for the assigned external applicaiton
          orchestratorLogicalName: # Password for basic authentication

## Outputs
 |Name|Description|
 |:--|:--|
 |analyzerResultsPath|A path on the local runner containing the analyzer result json files for all analyzed projects|
|analyzerResultsTable|Markdown formatted table containing the workflow analysis results, intended for use cases such as writing to the step summary and sending as a comment to a pull request|

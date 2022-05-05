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

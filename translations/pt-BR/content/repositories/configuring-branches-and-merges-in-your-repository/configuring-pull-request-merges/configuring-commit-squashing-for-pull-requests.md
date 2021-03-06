---
title: Configurar a combinação de commits por squash em pull requests
intro: 'Você pode aplicar, permitir ou desabilitar a combinação por squash do commit para todos os merges da pull request no {% data variables.product.product_location %} do seu repositório.'
redirect_from:
  - /articles/configuring-commit-squashing-for-pull-requests
  - /github/administering-a-repository/configuring-commit-squashing-for-pull-requests
  - /github/administering-a-repository/configuring-pull-request-merges/configuring-commit-squashing-for-pull-requests
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Repositories
shortTitle: Configurar combinação por squash de commit
---

{% data reusables.pull_requests.configure_pull_request_merges_intro %}

{% data reusables.pull_requests.default-commit-message-squash-merge %}

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
3. Under {% ifversion fpt or ghec or ghes > 3.4 or ghae-issue-6069 %}"Pull Requests"{% else %}"Merge button"{% endif %}, optionally select **Allow merge commits**. Isso permite que os contribuidores façam merge de uma pull request com um histórico completo de commits. ![allow_standard_merge_commits](/assets/images/help/repository/pr-merge-full-commits.png)
4. Under {% ifversion fpt or ghec or ghes > 3.4 or ghae-issue-6069 %}"Pull Requests"{% else %}"Merge button"{% endif %}, select **Allow squash merging**. Isso permite que os contribuidores façam merge de uma pull request combinando por squash todos os commits em um único commit. Se você selecionar outro método além de **Allow squash merging** (Permitir merge de combinação por squash), os colaboradores poderão escolher o tipo de commit do merge ao fazer merge de uma pull request. {% data reusables.repositories.squash-and-rebase-linear-commit-hisitory %} ![Commits de combinação por squash da pull request](/assets/images/help/repository/pr-merge-squash.png)

## Leia mais

- "[Sobre merges de pull request](/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/about-pull-request-merges)"
- "[Fazer merge de uma pull request](/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request)"

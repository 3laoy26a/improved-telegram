---
title: 为组织添加帐单管理员
intro: '*帐单管理员*是负责为组织管理帐单设置的用户管理员，例如更新付款信息。 如果组织的常规成员通常不能访问帐单资源，这将是一个很好的选择。'
redirect_from:
  - /articles/adding-a-billing-manager-to-your-organization
  - /github/setting-up-and-managing-organizations-and-teams/adding-a-billing-manager-to-your-organization
versions:
  fpt: '*'
  ghec: '*'
topics:
  - Organizations
  - Teams
  - Billing
shortTitle: 添加帐单管理员
---

组织所有者团队的成员可向人们授予*帐单管理员*权限。 在个人接受其邀请成为组织的帐单管理员后，他们可邀请其他人员为帐单管理员。

{% note %}

**注：**帐单管理员在组织的订阅中不使用付费许可。

{% endnote %}

## 帐单管理员的权限

帐单管理员可以：

- 升级或降级帐户
- 添加、更新或删除付款方式
- 查看付款历史记录
- 下载收据
- 查看、邀请和删除帐单管理员
- 开始、修改或取消赞助

此外，所有帐单管理员在组织的结算日期都会通过电子邮件收到结算收据。

帐单管理员**不**能：

- 在组织中创建或访问仓库
- 查看组织的私人成员
- 出现在组织成员列表中
- 购买、编辑或取消 {% data variables.product.prodname_marketplace %} 应用程序订阅

{% tip %}

**提示：**如果您的组织[要求成员、帐单管理员和外部协作者使用双重身份验证](/articles/requiring-two-factor-authentication-in-your-organization)，则用户必须启用双重身份验证后才可接受您的邀请，成为组织的帐单管理员。

{% endtip %}

## 邀请帐单管理员

{% ifversion ghec %}
{% note %}

**Note:** If your organization is owned by an enterprise account, you cannot invite billing managers at the organization level. 更多信息请参阅“[关于企业帐户](/admin/overview/about-enterprise-accounts)”。

{% endnote %}
{% endif %}

受邀人员将会收到邀请电子邮件，邀请他们成为您的组织的帐单管理员。 在受邀人员单击其邀请电子邮件中的接受链接后，他们会自动加入组织成为帐单管理员。 如果他们还没有 GitHub 帐户，将被重定向到注册页面注册一个，在创建帐户后会自动加入组织成为帐单管理员。

{% data reusables.organizations.billing-settings %}
1. 在“Billing management（帐单管理）”下的“Billing managers（帐单管理员）”旁边，单击 **Add（添加）**。 ![邀请帐单管理员](/assets/images/help/billing/settings_billing_managers_list.png)
6. 输入您要添加的人员的用户名或电子邮件地址，然后单击 **Send invitation（发送邀请）**。 ![邀请帐单管理员页面](/assets/images/help/billing/billing_manager_invite.png)

## 延伸阅读

- "[Inviting people to manage your enterprise](/enterprise-cloud@latest/admin/user-management/managing-users-in-your-enterprise/inviting-people-to-manage-your-enterprise)"{% ifversion fpt %} in the {% data variables.product.prodname_ghe_cloud %} documentation{% endif %}

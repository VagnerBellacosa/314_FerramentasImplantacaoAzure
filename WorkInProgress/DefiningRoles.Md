# Defining roles and responsibilities for cloud cost optimization

By [Omar Khan](https://azure.microsoft.com/en-us/blog/author/omar-khan/), General Manager, Azure Product Marketing

Share

- 
- 
- 

- Content type
- [Thought leadership](https://azure.microsoft.com/en-us/blog/content-type/thought-leadership/)

- Tag

more

Today’s challenging economic climate has driven many IT organizations to launch cost optimization initiatives. If you’re participating in one such initiative, you’ve discovered that cloud cost management is a journey, with many factors to consider and steps to take to improve cloud spending behaviors.

If you’re already running in the cloud, the best way to jumpstart your cost optimization initiative is by making sure you have the right governance in place, which will give you immediate cost benefits. Then you can circle back to the process outlined in the [Microsoft Cloud Adoption Framework for Azure](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/overview): define your cloud strategy, create your cloud adoption plan, ready your cloud environment, migrate and innovate cloud workloads, then manage and govern your environment. Each step of your cloud journey—from documenting your strategy to setting up ongoing operations—has a cost impact. Our [get started guide to managing cloud costs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/get-started/manage-costs) will help you understand the cost implications for each step along the way.

![Microsoft Cloud Adoption Framework for Azure](https://azure.microsoft.com/en-us/blog/wp-content/uploads/2020/12/fae01e65-6e4e-48a0-a4b5-91c13d2e712b.webp)

In this blog, we’re zooming in on the first step—governance—to help you hit the ground running. We’ll outline best practices, both in assigning roles and responsibilities to your teams, and how those teams should take joint action to create a more cost-efficient cloud environment.

## The three key teams involved in cost management

You might call them by slightly different names or have a slightly different organizational model ([team structure is a journey too](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/organize/organization-structures)), but fundamentally, based on our conversations with customers who are having the most success managing costs, there should be three key teams involved in cost management and optimization:

1. The **cloud strategy team** defines motivations and business outcomes for cloud investments and aligns business priorities and cloud adoption efforts.
2. The **cloud governance team** mitigates the risks associated with cloud investments by converting those risks into sound corporate policies.
3. **Cloud adoption teams** (or **cloud workload teams**) implement technical solutions in the cloud to deliver on the cloud strategy, in alignment with policy.

Fundamentally, these teams play the following roles in a cost-conscious organization:

- The **cloud strategy team** builds cost consciousness into cloud efforts at the leadership level, for example, by establishing budgets and reviewing spend and return on investment (ROI) across cloud investments.
- The **cloud governance team** manages costs across the cloud portfolio, for example, delivering reliable cost reporting and performance telemetry, and optimizing the cloud environment to address budget deviations.
- The **cloud adoption teams** (or **cloud workload teams**) serve as the first lines of defense against overspending by understanding cost goals and how their implementation decisions affect those and by collaborating with the cloud governance team to optimize workloads.

To learn more about these teams and their core cost management responsibilities, [see our documentation](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cost-conscious-organization).

## Operational cost management best practices

There are areas of cost management where the cloud governance team takes the lead, areas where the cloud adoption teams (or cloud workload teams) take the lead, and areas of close collaboration among them.

Typically, the cloud governance team is responsible for [operational cost management best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/cost-management/best-practices#operational-cost-management-best-practices), for example, patching and maintenance. This set of best practices is usually handled centrally. Examples include:

- **Tagging**: Ensuring all your cloud resources are tagged properly.
- **Licensing**: Leading a well-planned license acquisition and utilization strategy, including taking advantage of the Azure Hybrid Benefit, Azure Reservations, Azure Spot Virtual Machines, and other buying strategies that can rapidly reduce costs across your entire cloud portfolio.
- **Bulk shutdowns**: Identifying large numbers of resources that are no longer being used and working with owners to shut them down.
- **Bulk right-sizing**: Finding mass opportunities for right-sizing resources to the smallest stock-keeping units (SKUs) that can support performance requirements.

We provide [tools to help you follow these best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/cost-management/toolchain). For example, you can establish, audit, and enforce proper resource tagging with [Azure Policy](https://azure.microsoft.com/en-us/services/azure-policy/), and find a list of opportunities to shut down and right-size resources with [Azure Advisor](https://azure.microsoft.com/en-us/services/advisor/). [Azure Cost Management and Billing](https://azure.microsoft.com/en-us/services/cost-management/) gives you a full set of cloud cost management capabilities so you can better understand and control your spending.

## Workload cost management best practices

The cloud adoption team (or cloud workload team) is typically responsible for following [workload-level cost management best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/cost-management/best-practices#workload-cost-management-best-practices). The cloud workload team might consult with the cloud governance team (or receive training or coaching from them), or handle these items independently. These best practices include:

- **Granular re-sizing and shutdown**: Finding more nuanced opportunities (beyond those large-scale opportunities identified by the central cloud governance team) to shift resource SKUs or shut down resources altogether.
- **Horizontal-over-vertical scale**: Using multiple small instances rather than fewer large instances to scale, often resulting in cost efficiencies.
- **Autoscaling**: Taking advantage of automation to more closely match workload demand to resource counts and sizes.
- **Revising architecture**: Revisiting early architectural decisions for cost efficiencies, such as through serverless technologies.

To guide decisions in this area, we recommend consulting the [Microsoft Azure Well-Architected Framework](https://docs.microsoft.com/en-us/azure/architecture/framework/), which can help you design, build, deploy, and manage high-quality cloud workloads across five key pillars: security, reliability, performance efficiency, operational excellence, and cost optimization. To get started, check out the [Microsoft Azure Well-Architected Review](https://docs.microsoft.com/en-us/assessments/?id=azure-architecture-review&mode=pre-assessment), which you can use to assess your workloads against the Well-Architected Framework, including the cost optimization pillar. The Well-Architected Review provides a holistic view into cost optimization guidance for your deployed workloads, and actionable recommendations to help you optimize them. You can also utilize the tools referenced above, like [Azure Advisor](https://azure.microsoft.com/en-us/services/advisor/) to get real-time recommendations for your deployed Azure resources.

## Working towards a cost-conscious organization

Creating a cost-conscious organization that delivers on your financial goals is a team sport. Everyone has a role to play to ensure you meet your business objectives. Learn more about the [teams responsible for cost management](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cost-conscious-organization) and the [best practices each of these teams should follow](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/cost-management/best-practices). Then get started optimizing today.

Stay tuned for more on how to manage your cloud spending, so you can focus on what matters most to your business. Meanwhile, visit our [cost optimization site](https://azure.microsoft.com/en-us/overview/cost-optimization/) for more resources.
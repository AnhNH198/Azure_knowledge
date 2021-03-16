* a tenant is associated with a single identity (person, company, or organization) and can own one or several subscriptions


* a subscription is linked to a payment setup and each subscription will result in a separate bill
in every subscription, you can add virtual resources (VM, storage, network, ...)

### Additionally:
* Every tenant is linked to a single Azure AD instance, which is shared with all tenant's subscriptions

* Resources from one subscription are isolated from resources in other subscriptions

* An owner of a tenant can decide to have multiple subscriptions:

### When Subscriptions limits are reached

* to use different payment methods
* to isolate resources between different departments, projects, regional offices, and so on.


### Example 1:
Contoso decides to have **a tenant** with 2 subscriptions:

one subscription for the Prod department with Credit Card A
one subscription for the Dev department with Credit Card B

(but could also be the same Credit Card as the one of another subscription)
In this example, the two departments **share the same Azure AD database**. However, **resources are isolated between departments, and budgets can be separated too**.

### Example 2:
A holding company decides to have 2 tenants:

one tenant for subsidiary Contoso with one subscription for Dev and Prod
one tenant for subsidiary Fabrikam with one subscription for Dev and another subscription for Prod
In this example, both companies have a different Azure AD database.

### Example 3:
You have a tenant for your personal training.
In this tenant, you can have:

1. one free Azure subscription (linked to a credit card but not charged, and can be converted to a Pay-As-You-Go subscription after the free trial)
2. one or several Pay-As-You-Go subscriptions (linked to different credit cards)
3. one or several Azure Pass Sponsorship subscriptions, not linked to any credit card because these subscriptions are obtained during Microsoft trainings
4. one Visual Studio subscription (linked to a credit card) and with different quotas (of free resources) than the free subscription

Despite all those subscriptions have isolated resources (per subscription), and some are free while you have to pay for others, all subscriptions share the same Azure AD database.
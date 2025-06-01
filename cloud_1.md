
# Network Design

## 4.2.1 Cloud Server

## Estimations

  1. Azure:
    - Region: Australia East
    - Operating System: Windows Server
    - CPU: 4 vCPUs
    - Memory: 16 GB RAM
    - Storage: 100 GB SSD
    - Price: AUD $150/month
    - Link: [Azure Pricing Calculator](https://azure.microsoft.com/en-us/pricing/calculator/)

  2. AWS:
    - Region: Asia Pacific (Sydney)
    - Operating System: Windows Server
    - CPU: 4 vCPUs
    - Memory: 16 GB RAM
    - Storage: 100 GB SSD
    - Price: AUD $140/month
    - Link: [AWS Pricing Calculator](https://calculator.aws/)

  3. Google Cloud:
    - Region: Sydney
    - Operating System: Windows Server
    - CPU: 4 vCPUs
    - Memory: 16 GB RAM
    - Storage: 100 GB SSD
    - Price: AUD $130/month
    - Link: [Google Cloud Pricing Calculator](https://cloud.google.com/products/calculator)

  b. Recommendation:

    Based on the estimates, I recommend using Google Cloud for the following reasons:
    1. Competitive Pricing: Google Cloud often provides competitive pricing compared to Azure and AWS.
    2. Performance: Google Cloud's infrastructure is known for its high performance and reliability.
    3. Integration: Google Cloud offers seamless integration with other Google services, which can be beneficial for future expansion.

  c. Total Cost Calculation:
      [cloud_service_price_in total_estimate](cloud_service_price_estimate.xlsx)
    - To calculate the total cost of using all cloud VMs to replace the existing servers over a 3-year period,
    we'll sum up the costs for three servers at headquarters and one server per branch office (total of six servers).

  d. Total Cost for Google Cloud VMs:
    - Monthly Cost per VM: AUD $130
    - Number of VMs: 6
    - Monthly Cost for all VMs: 130 * 6 = AUD $780
    - Annual Cost for all VMs: 780 * 12 = AUD $9,360
    - Total Cost for 3 Years: 9,360 * 3 = AUD $28,080

  e. Disadvantages of Cloud VMs:

    - Dependency Reliance on the cloud provider for uptime and performance.
    - Security Potential concerns about data security and privacy.
    - Internet Connectivity Requires stable and high-speed internet connection for optimal performance.


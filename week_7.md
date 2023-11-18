# Project_Alpha

## Week 7

### Route 53

#### Task 1: Register a Domain (if not done already):
- If you haven't registered a domain yet, you can do so through Route 53 or another domain registrar.
- If using a different registrar, you may need to update the name servers to point to Route 53.

#### Task 2: Create a Hosted Zone:
- In Route 53, create a hosted zone for your domain. This is where your DNS records will be stored.

#### Task 3: Get Name Servers:
- Note the name servers provided by Route 53 for your hosted zone. You'll need to update this information with your domain registrar.

#### Task 4: Update Name Servers at Domain Registrar:
- Log in to your domain registrar's website and update the name servers to the ones provided by Route 53. This delegates DNS management to Route 53.

#### Task 5: Add DNS Records:
- Inside your hosted zone, add the necessary DNS records (e.g., A records, CNAME records, MX records) to define how traffic is routed for your domain and its subdomains.

1. **Task 5.1: Create A Records for Web Hosting**:
If you are hosting a website, create A records that point to the IP address of your web server.

2. **Task 5.2: Create CNAME Records**:
For services like Amazon S3, CloudFront, or other AWS resources, create CNAME records to associate your domain/subdomain with the corresponding AWS resource.

3. **Task 5.3: Create MX Records for Email**:
If you are using Route 53 for email, create MX (Mail Exchange) records to specify mail servers responsible for receiving email messages.

4. **Task 5.4: TTL (Time to Live) Configuration**:
Set the TTL for your DNS records. TTL determines how long DNS resolvers should cache the information before querying the authoritative DNS servers again.

#### Task 6: Verify DNS Configuration:
- After setting up your DNS records, use DNS lookup tools or services to verify that your records are resolving correctly.

#### Task 7: Enable DNSSEC (optional):
- If you want to add an extra layer of security, consider enabling DNS Security Extensions (DNSSEC) for your domain.

#### Task 8: Monitor and Maintain:
- Regularly monitor your DNS settings, especially when making changes to your infrastructure. Ensure that records are up to date and accurately reflect your current setup.

  [Route 53 Documentation](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html)

### CloudFront

#### Task 1: Create a Distribution:
- Access the CloudFront console in the AWS Management Console.
- Click on "Create Distribution" to initiate the distribution creation process.

#### Task 2: Configure Origin:
- Choose an AWS origin or input your origin's domain name.
- Optionally, set an origin path and name for this origin.
- Add custom headers if needed.
- Enable or disable Origin Shield for additional caching.

#### Task 3: Configure Default Cache Behavior:
- Set the default cache behavior, including path patterns and automatic object compression.
- Specify the viewer protocol policy and allowed HTTP methods.
- Optionally, restrict viewer access using signed URLs or cookies.

#### Task 4: Cache and Origin Request Policies:
- Use recommended cache and origin request policies for better control.
- Choose or create cache and origin request policies as needed.
- Optionally, configure response headers policy.

#### Task 5: Function Associations (Optional):
- Associate edge functions with specific CloudFront events (Viewer request, Viewer response, Origin request, Origin response).

#### Task 6: Web Application Firewall (WAF):
- Enable or disable security protections using AWS WAF.
- Select included security protections based on your application's needs.

**Price Estimate:**
Review the estimated cost for the AWS WAF configuration.

- <!-- To be covered in the next subtopic below -->
- *Will delve into detailed WAF configuration in the upcoming subtopic.*

#### Task 7: Settings:
- Choose the price class based on desired edge location coverage.
- Optionally, add alternate domain names (CNAMEs) and associate a custom SSL certificate from AWS Certificate Manager.
- Specify supported HTTP versions and set the default root object.
- Decide on standard logging, IPv6 support, and provide an optional description.

#### Task 8: Create Distribution:
- Click "Create Distribution" to initiate the distribution creation process.

#### Task 9: Post-Creation Steps:
- Monitor the distribution deployment status.
- Update DNS settings for your domain to point to the CloudFront distribution.
- Test the distribution after DNS changes have propagated.

#### Task 9: Optimize and Monitor:
- Regularly monitor CloudFront metrics, logs, and optimize cache settings based on performance and usage patterns.

[AWS CloudFront documentation](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html)

### Web Application Firewall

#### Task 1: Explore the New AWS WAF Dashboards:
- Log in to the AWS Management Console and navigate to the AWS WAF console.
- Explore the updated AWS WAF dashboards by choosing one of your web ACLs.
- These enhanced dashboards offer a more user-friendly interface for effective management and monitoring of your WAF configurations.

#### Task 2: Create a Web ACL:
- If no existing Web ACL is present, initiate the creation of a Web Access Control List (Web ACL) by selecting "Create web ACL."
- Proceed to provide a name and description for the new Web ACL during the configuration process.

#### Task 3: Configure Web ACL Settings:
- Follow the prompts to configure settings for the Web ACL.
- Explore options such as IP sets, Regex pattern sets, and Rule groups to define conditions and actions.

#### Task 4: Explore Application Integration:
- Check out the new Application Integration section for additional features and integrations to enhance your WAF setup.

#### Task 5: Manage Web ACLs:
- Use the Web ACLs tab to view and manage your existing Web ACLs.
- Copy the ARN (Amazon Resource Name) for reference or delete any obsolete Web ACLs.

#### Task 6: Switching to AWS WAF Classic:
- If you have web ACLs created in the AWS WAF Classic console, you can access them by clicking the provided link.
- Note that resources created under AWS WAF Classic aren't compatible with the new AWS WAF.

#### Task 7: AWS Shield Integration:
- Explore AWS Shield features by navigating to the AWS Shield section.
- Understand the overview, protected resources, events, and the global threat dashboard.

#### Task 8: AWS Firewall Manager:
- Check out AWS Firewall Manager features, including security policies, application lists, and protocol lists.

#### Task 9: Documentation and Support:
- Access CloudShell and provide feedback on the AWS WAF interface.
- Refer to AWS documentation for detailed guides and support.
[AWS WAF Documentation] (https://docs.aws.amazon.com/waf/)

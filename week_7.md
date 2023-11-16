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
Log in to your domain registrar's website and update the name servers to the ones provided by Route 53. This delegates DNS management to Route 53.

#### Task 5: Add DNS Records:
Inside your hosted zone, add the necessary DNS records (e.g., A records, CNAME records, MX records) to define how traffic is routed for your domain and its subdomains.

1. **Task 5.1: Create A Records for Web Hosting**:
If you are hosting a website, create A records that point to the IP address of your web server.

2. **Task 5.2: Create CNAME Records**:
For services like Amazon S3, CloudFront, or other AWS resources, create CNAME records to associate your domain/subdomain with the corresponding AWS resource.

3. **Task 5.3: Create MX Records for Email**:
If you are using Route 53 for email, create MX (Mail Exchange) records to specify mail servers responsible for receiving email messages.

4. **Task 5.4: TTL (Time to Live) Configuration**:
Set the TTL for your DNS records. TTL determines how long DNS resolvers should cache the information before querying the authoritative DNS servers again.

#### Task 6: Verify DNS Configuration:
After setting up your DNS records, use DNS lookup tools or services to verify that your records are resolving correctly.

#### Task 7: Enable DNSSEC (optional):
If you want to add an extra layer of security, consider enabling DNS Security Extensions (DNSSEC) for your domain.

#### Task 8: Monitor and Maintain:
Regularly monitor your DNS settings, especially when making changes to your infrastructure. Ensure that records are up to date and accurately reflect your current setup.

  [Route 53 Documentation](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html)


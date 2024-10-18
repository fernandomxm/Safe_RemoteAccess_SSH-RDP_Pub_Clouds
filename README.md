Como melhor prática de segurança, é necessário que não se utilize a liberação de acesso dos protocolos SSH e RDP nos security groups para acesso remoto para gerenciamento de instâncias.

Segue abaixo, qual a forma mais segura de se fazer este acesso remoto em cada cloud provider:


AWS - Utilize Instance Connect Endpoint (https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connect-using-eice.html)

Obs: Se a instância NÃO POSSUI IP Público associado ou não tenha acesso liberado para internet

https://youtu.be/8U9OSHf06uM

AWS - Utilize o Session Manager (https://docs.aws.amazon.com/pt_br/systems-manager/latest/userguide/session-manager.html)

Obs: Se a instância POSSUI IP Público associado ou acesso liberado para navegação

https://youtu.be/nt6NTWQ-h6o

GCP - Utilize IAP(Identity-Aware Proxy) (https://cloud.google.com/iap?hl=pt_br)

OCI - Utilize Bastion Host (https://www.oracle.com/br/security/cloud-security/bastion/)

AZURE - Utilize Bastion Host (https://azure.microsoft.com/en-us/products/azure-bastion)

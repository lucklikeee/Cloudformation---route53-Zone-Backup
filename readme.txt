Template cloudormation para backup de todas as zonas de dns da conta:


Backup a cada 12 horas (cron 0 0/12 * * ? *)

Todas as zonas Route53 serão exportadas para zone files BIND

S3 bucket criado (nome definido no template)

Ciclo de vida avançado:

Menos de 30 dias → Standard

60–90 dias → GLACIER, excluídos após 90 dias

Lambda + Role + EventBridge integrados

Скрипт ssl_valid_days.sh скопирован с  https://blog.sleeplessbeastie.eu/2017/04/03/how-to-display-days-till-certificate-expiration/.

Шаблон содержит:
  - Макросы:\
  {$DOMAINS_LIST_FILE} - путь до файла с именами доменов в формате JSON;\
  {$WARN_DAYS} - Количество дней до истечения времени действия сертификата.
  
  - Правило обнаружение: \
  ssl_cert_check_list - получает содержимое файла {$DOMAINS_LIST_FILE}. 
  
  - Прототип элементов данных:  \
  {#DOMAIN} ssl valid days - количество дней до истечения срока действия сертификата. 
  
  - Прототип триггеров:  \
  {#DOMAIN} ssl valid days < {$WARN_DAYS}. 


Script ssl_valid_days.sh downloaded from  https://blog.sleeplessbeastie.eu/2017/04/03/how-to-display-days-till-certificate-expiration/.

Template have macroses:\
{$DOMAINS_LIST_FILE} - path to domains list file;\
{$WARN_DAYS} - Days count for the trigger.

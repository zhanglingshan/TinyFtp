## Tinyftpd
----------
### ����
Tinyftpd����c����ʵ�ֵļ򵥡����١���Ч��Linux FTP��������ֻ��򵥵����ã��Ϳɿ��ٵĽ�������ɸ�Ч��FTP��������

### ģ����
TinyFTP��Ϊ �ַ�������ģ�顢��������ģ�顢socketģ�顢�ڲ����̼�ͨѶģ�顢ϵͳ���ù���ģ�顣

1. �ַ�������ģ�飺�ַ���ģ����Ҫ���������������У����ֶ��ַ����Ĵ���ģ����`string.h` �� `string.c`
2. ��������ģ�飺��������ģ���ṩ�������õĹ��ܡ�������`parseconf.h` �� `parseconf.c` 
3. socketģ�飺����socketͨѶ���������ݴ��䡣�ɼ� `commonsock.h` `commonsock.c`
4. �ڲ����̼�ͨѶģ�飺�����ӽ��� �� �����̼��ͨѶ �����ݴ��䡣`privsock.h` �� `privsock.c`
5. ϵͳ���ù���ģ�飺��Ҫ��һЩ�õ���ϵͳ���õĺ�����װ���ɼ�`sckutil.h` `sckutil.c`

### ��װ
#### ����
```bash?linenums=NULL
cd build/
chmod +x bulid.sh
sudo ./build.sh
```
����
```bash?linenums=NULL
cd /bin
sudo ./tinyftpd
```

### ����
�����ļ��ڵ�ǰĿ¼��`tinyftpd.conf`

|       ���ò���                |    ˵��        |
| ------------------------------| ---------------|
|tunable_pasv_enable 	        |�Ƿ�������ģʽ|
|tunable_port_enable 	        |�Ƿ�������ģʽ|
|tunable_max_clients 	        |���������      |
|tunable_max_per_ip 	        |ÿIP���������  |
|tunable_listen_port	        |FTP�������˿�   |
|tunable_accept_timeout 	    |accept��ʱ��    |
|tunable_connect_timeout	    |connect��ʱ��   |
|tunable_idle_session_timeout	|����ʱ�����ӳ�ʱ|
|tunable_data_connection_timeout|��������ʱ�䳬ʱ|
|tunable_local_umask	        |����            |
|tunable_upload_max_rate 	    |����ϴ��ٶȣ�byte/s��|
|tunable_download_max_rate 	    |��������ٶȣ�byte/s��|
|tunable_listen_address	        |FTP������IP��ַ |

### LICENSE
�����ѭMIT��ԴЭ��
### ��л
�ڿ��������вο���vsftpd��Դ�룬����ѧ�������֪ʶ���ش���������ʾ��л
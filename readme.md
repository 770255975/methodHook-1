#��װ���������̣�
* ��Ҫһ̨root����android4.4.x���豸
* �ڸ��豸�а�װXposed Installer�ͻ��ˣ����ڰ�װXposedʱ����Ҫ��android��app_main.cpp���ļ������滻��     
������Ҫandroid��rootȨ��
* ��װ��д�õ�com.bingpang.methodhookģ�����ÿͻ��ˣ���ʱXposed�ͻ��˽����⵽��Xposedģ�飬��ͼ��ʾ    
![��װģ���ͼ](moban.png)
* ��ѡ��ģ�岢����android�豸
----
----
----
#Hook Method����
##ʵ�ֵĹ���
* ��ǩΪFM��log����˾������к�������ͷ���������android.telephony.SmsManager->sendTextMessage
* ��ǩΪDetailInform��log����������к�����Ӧ�����ݣ�����android.telephony.SmsManager->sendTextMessage��      
�����Send SMS -> SMS DestNumber: destNumber , SMS Content: Content      
##��������к����б�
*SmsManager*
1. android.telephony.SmsManager/sendTextMessage
2. android.telephony.SmsManager/getAllMessagesFromIcc
3. android.telephony.SmsManager/sendDataMessage
4. android.telephony.SmsManager/sendMultipartTextMessage
*TelephonyManager*
1. android.telephony.TelephonyManager/getLine1Number
2. android.telephony.TelephonyManager/listen
*AccountManager*
1. android.accounts.AccountManager/getAccounts
2. android.accounts.AccountManager/getAccountsByType
*ActivityManager*
1. android.app.ActivityManager/killBackgroundProcesses
2. android.app.ActivityManager/forceStopPackage
*AlarmManager*
1. android.app.AlarmManager/setImpl
*AudioRecord*
1. android.media.AudioRecord
*Camera*
1. android.hardware.Camera/takepicture
2. android.hardware.Camera/setPreviewCallback
3. android.hardware.Camera/setPreviewCallbackWithBuffer
4. android.hardware.Camera/setOneShotPreviewCallback
*ConnectivityManager*
1. android.net.ConnectivityManager/setMobileDataEnabled
*ContentResolver*
1. android.content.ContentResolver/qurey
2. android.content.ContentResolver/registerContentObserver
3. android.content.ContentResolver/insert
4. android.content.ContentResolver/bulkInsert
5. android.content.ContentResolver/delete
6. android.content.ContentResolver/update
7. android.content.ContentResolver/applyBatch
*ContextImpl*
1. android.app.ContextImpl/registerReceiver
*MediaRecorder*
1. android.media.MediaRecorder/start
2. android.media.MediaRecorder/stop
*Internet*
1. java.net.URL/openConnection
2. org.apache.http.impl.client.AbstractHttpClient/execute
*NotificationManager*
1. android.app.NotificationManager/notify
*ApplicationPackageManager*
1. android.app.ApplicationPackageManager/installPackage
2. android.app.ApplicationPackageManager/deletePackage
3. android.app.ApplicationPackageManager/getInstalledPackages


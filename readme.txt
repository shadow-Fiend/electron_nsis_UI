1. Ŀǰ���õ�NSIS��Unicode�汾  �����ڿ���̨���������Ļ���һ�����ţ����ù���

@rem ���Ҫ���Դ�����ʹ������Ľű���������򿪱�����棨�����н������Ļ���ʾ��?�ţ�
".\NSIS\makensisw.exe" xxx


2. ��skinĿ¼�����ý���

3. nsi�ļ������ð�װ�������Ϣ �����İ�װ�߼���commonfunc.nsh�Լ���nsi�ļ���һ��� nsh�ļ���

4. �нӿڲ����׵ģ���ο�ʾ���Լ��ĵ�����  

5. ���е�nsis��nsi�Լ� nsh�ļ�����Ҫ��unicode����utf-8���� 

6. ����ShowMsgBox�ӿڣ�������һ������������ָ����������ʹ�õ���ʽ�ļ������磺
nsNiuniuSkin::ShowMsgBox "notice title" "notice message." 0 "msgBox2.xml"
�������ʹ��msgBox2.xml����������ʽ����ʾ���ڣ����ڸ��Ի�������ʾ��������  

8. Ҫʹ��rtf�ļ���Ϊ���Э���ļ�����Э���ļ��ĳ�rtf���ɣ��ο�nimʾ����

9. �ɰ汾����������Ŀ����Ҫ�޸�ԭ����install.xml�е�Font�ڵ㣬������������ָ��Font��idֵ�������0��ʼ����ԭ������������������Լ��ݾɵ����ã�
10.�����������ѷ�����װ���б�����������밴���·�ʽ����
ͨ��ִ��setup.exe����Ҫǩ������������ж�س���Ȼ���ж�س������ǩ�����ٽ�ж�س�������setup.exe��
1�����ȣ���NSIS����setup.exe��ע�⣺��Ҫ��setup.exe����ǩ����
2��ִ��setup.exe������װ��ɺ󣬵���װĿ¼�ҵ�uninst.exe��Ȼ���uninst.exe����ǩ����
3����uninst.exe�ļ�����Ҫ���ͷŵ���װĿ¼�µ��ļ�һ���� (�ŵ�FilesToInstallĿ¼��)��
4��ע�͵�commonfunc.nsh�ļ��е���䣺WriteUninstaller "$INSTDIR\uninst.exe"��
5�����±���setup.nsi����setup.exe�����������ǩ����

10. Ϊ�������ؼ��Ŀ���չ�ԣ��ؼ�2.0�汾�Խӿڽ�����ȫ��������Ӽ�������ʹ���°汾�ӿڣ�20171210����
1) ȥ����SetDirValue��GetDirValue��GetCheckBoxStatus��SetSliderValue��SetSliderRange�Ⱥ���������ʹ��ͨ�õ�SetControlAttribute�Լ�GetControlAttribute�����û��ȡ 
2) ȥ����ԭ����ShowDlgBox�ӿڣ�����Ϊ��ʹ��nsNiuniuSkin::InitSkinSubPage����ʼ���������Ӵ��ھ����Ȼ��ʹ��nsNiuniuSkin::ShowSkinSubPage��ʽ��ʵ�� 
  �����ַ�ʽ�������̶ȵ������Ӵ��ڵĿ���չ�ԣ�UI�������ⶨ���ˣ����ܿؼ�ID�ŵ��κ����ƣ�
3) �����е���UI��صĽӿڣ�������һ������������Ա��ܹ�ʹ��һ���ӿھͿɿ����������Լ��Ӵ��ڵĸ������Ե��������ȡ  
4) ��һ��������UI�ؼ��ڲ����ڹ̶��ؼ�ID�����ã������ű��Ŀɿ�����

�ο���ַ��
http://blog.csdn.net/hellokandy/article/details/52212495
git��ʼ��
����ȫ���û���Ϣ���ֲ�ʽ�汾���ƣ�  
$ git config  --global user.name  ���û�����  
$ git config --global  user.email  �����䡱  
����Ĭ�ϵı༭��  
$ git config --global core.editor "�༭�����г����·��"  
�鿴git��������Ϣ  
$ git config --list  
�鿴git�������ֲ�  
$ git help  

Git�ֿ⣨repository��  
��ʼ���汾�⣺git init  
����ļ����汾��  
$git add  �ļ���  
$git commit  -m "�ύ��˵��"  
�鿴git�ֿ�״̬  
$git status  

���Զ�ֿ̲�  
$git remote add origin http��ַ  
��һ���ύ��ʱ���Ĭ�ϴ���master��֧(pwd չʾ��ǰĿ¼��Ϣ,mkdir �����ļ���)  
���͵�Զ��  
$git push  
�����Ŀ������(Ĭ�ϰѷ�֧�Ѿ���Զ�˹�����)  
$git clone http��ַ  

�ص���ȥ  
���汾�������ݸ��ǵ��ݴ���������������仯�����Ҫʹ�������仯��  
$git reset head  
���汾�����������ã����桢�汾�⡢���ض���仯��  
$git reset  --hard hash�� 
��ձ����ļ�    
$git rm �ļ���  

��ǩ����������̱���  
�鿴���б�ǩ�� $git tag  
������ǩ��$git tag name  
ָ���ύ��Ϣ:git tag -a name -m "comment"   
ɾ����ǩ:git tag -d name (ɾ����ǩ��Ϊ)  
��ǩ������git push origin name  

��֧����  
git branch name ����name�ķ�֧  
git checkout name �л���֧  
git branch �鿴��֧���鿴��ǰ���ĸ���֧��  
�л���master��֧�ϣ�git checkout master 
*�����������Ǹ���֧��  
�ϲ���֧���뵽master����Ҫ�Ȱѷ�֧�л���master��֧�ϣ���git merge ��֧��  
ɾ����֧���ϲ���֧�󣬷�֧��û�����ã���git branch -d ��֧��  

������  
Git ������״̬������ļ����ܴ�������֮һ�����ύ��committed�������޸ģ�modified�������ݴ棨staged���� ���ύ��ʾ�����Ѿ���ȫ�ı����ڱ������ݿ��С� ���޸ı�ʾ�޸����ļ�������û���浽���ݿ��С� ���ݴ��ʾ��һ�����޸��ļ��ĵ�ǰ�汾���˱�ǣ�ʹ֮�������´��ύ�Ŀ����С�
�ɴ����� Git ��Ŀ��������������ĸ��Git �ֿ⡢����Ŀ¼�Լ��ݴ�����

����GitHUbԶ�ֿ̲�
ssh-keygen -t rsa -C "ע�������"   
ssh -T git@github.com �жϱ��زֿ��Զ�ֿ̲��Ƿ���ͨ    
git remote add origin git@github.com "���Զ�ֿ̲�"  
git push -u origin master "��һ������Զ�ֿ̲�����"��Ĭ�ϰѱ���master��Զ��master������   
git pull origin <��֧��> "��Զ�̷�֧��ȡ���������أ�ͬʱ�ѱ��ش����Զ�̴���ϲ�  
origin һ����Դ����Ϊ��Զ�ֿ̲�  

�ܽ�
�������� �������������ݴ����������汾��  
��ʼ��  git init ������git add ������gitcommit  
Զ�ֿ̲⣺Git remote add ����>git pull(��ȥ���µĴ���)������git push ����>git clone  
��֧����git branch ����>git checkout  

���ڶ��˺����ľ���  
  ���ÿͻ��˺͹��ߣ����������У�������Linux��������ֱ�ӿ���  
  ÿ���ύǰ��diff�Լ��Ĵ��룬�����ύ����Ĵ���  
 �°�ؼ�ǰ������Լ��Ĺ�������  
 ���е���Ŀ��ʹ�÷�֧����  
 ������ͻʱ�������׳�ͻ��ԭ��ǧ��Ҫ���ⶪ�����˵Ĵ���  
 ��Ʒ�����󣬼ǵô�Tag����ò�֪�����ϵİ汾�����㽫������֧�޸�BUG  
 ����ǰʹ��git pull�ϲ�Զ�̱仯�Ĵ���  

������Ϣ
Ls -a �����غͲ����ص��ļ�����ʾ  
Echo "git repo2" >> text.txt �ܵ�׷��(>>׷�ӣ�echo�����)  

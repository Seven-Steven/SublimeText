### �״α���
1. �򿪰�װ�õ� Sublime Text��ѡ�� ���˵����� ���� ��Preferences�� ���� ��Browse Packages�� �� Sublime Text �����ļ�Ŀ¼��
 > Windows ��һ����: `C:\Users\${your_username}\AppData\Roaming\Sublime Text 3\Packages`
 <!-- > Linux ��һ����: `` -->
2. �ر� Sublime Text �����
2. ���� **User** Ŀ¼������ **.gitignore** �ļ�������Ϊ��
```
Package Control.last-run
Package Control.ca-list
Package Control.ca-bundle
Package Control.system-ca-bundle
Package Control.cache/
Package Control.ca-certs/
```
�������Ŀ�ǲ���Ҫͬ�����ļ�/�ļ��У��ɸ���ʵ�����������
3. �� GitBash������ִ���������
```
git init # ��ʼ�� git �ֿ�
git add . # ���ٱ����ļ�
git commit -m "${comment}" # �ύ���θ��£����У�${comment} �Ƕ��ڱ����ύ��˵��
git remote add origin ${your_github_repository} # ���Զ�ֿ̲�
git push origin master # �ύ���ر����Զ�ֿ̲�
```
���ˣ�sublime text �Ĳ���Լ����ñ�����ϣ�
### �״λָ�
1. �ڵ�ǰ�ն˰�װ���� sublime text �����
2. ѡ�񡰲˵����� ���� ��Preferences�� ���� ��Browse Packages�� �� Sublime Text �����ļ�Ŀ¼��
3. �ر� Sublime Text �����
3. �� git bash������ִ���������
```
mv User User.old # ����
git clone ${your_github_repository} User # ��¡Զ�ֿ̲⵽���� User Ŀ¼
```
5. �� Sublime Text����װ Package Control
  * ���� `ctrl` + `~` ������ѡ�� ���˵����� ���� ��View�� ���� ��Show Console�� �򿪿���̨��
  * ������������ճ���� Sublime ����̨���س�ִ�У�
  ```
  import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
  ```
  ������ [Installation - Package Control](https://packagecontrol.io/installation) ��ѯ�������
  * �ȴ�����ִ�����
6. �ָ���ϣ�
### �ճ����ݻָ�
1. �������һ���ն����������Ķ����� `${package_folder}/User` Ŀ¼��ִ��
```
git add .
git commit -m "${comment}"
git push origin master
```
���ɡ�
2. �����Ҫ�ָ������ն˵����ø��£��� `${package_folder}/User` Ŀ¼��ִ��
```
git pull origin master
```
���ɡ�
### ����嵥
����һ�����Լ�ʹ�õĲ���嵥���Ͳ��������������
  1. Package Control
  1. Alignment
  1. BracketHighlighter
  1. Color Highlighter
  1. ConvertToUTF8
  1. CSS Comments
  1. DocBlockr
  1. Emmet
  1. HTML5
  1. MarkdownEditing
  1. MarkdownPreview
  1. PlainTasks
  1. SideBarEnhancements

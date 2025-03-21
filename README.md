 공격자가 웹 서버의 디렉터리 구조를 파악하기 위해 시도하는 공격입니다. 취약한 웹 서버는 디렉터리의 내용을 노출시킬 수 있으며, 공격자는 이를 통해 중요 파일이나 취약점을 찾아 악용할 수 있습니다.
- 대응 방법: 웹 서버 설정에서 디렉터리 리스팅 기능을 비활성화하고, `.htaccess` 파일 또는 웹 방화벽 규칙을 사용하여 `fckeditor/` 와 같은 특정 경로에 대한 접근을 차단합니다.
FCKeditor는 게시판 에디터입니다.
거의 모든 브라우저에서 사용 가능한 에디터로서, 글작성 / html편집 /표삽입 등이 가능합니다.
현재 FCKeditor는 3.x 대로 업그레이드 되면서 CKeditor로 변경되었으나,
아직 많은 곳에서 FCKeditor를 사용하고 있습니다.
공식사이트 : http://ckeditor.com
FCkeditor 2.6.11 Ver : http://sourceforge.net/projects/fckeditor/files/
 

 
 
------------------------------------------------------------------------------------------------------------------------------------------
2. 취약점 발생 원인
------------------------------------------------------------------------------------------------------------------------------------------
취약점이 발생하는 이유는 FCKeditor에서 제공되는 페이지관리 또는 파일업로드 기능때문입니다.
해당 기능을 사용할 수 있는 페이지에 적절한 보안조치가 이루어지지 않으면
웹쉘이 업로드되거나 홈페이지의 많은 정보가 노출될 수 있습니다.
 
아래 그림은 FCKeditor 2.6.11 버전의 기본 경로입니다. 

## xcode에서 한글로 Key Binding
xcode 14부터 xcode - settings - Key Bindings에서 키보드를 한글로 변경하면 shortcut 등록이 안됨
Key Bindings 파일에 직접 등록하는 방식으로 해결
~/Library/Developer/Xcode/UserData/KeyBindings/Default.idekeybindings
파일 실행 후 
```XML
	<key>Text Key Bindings</key>
	<dict>
		<key>Key Bindings</key>
		<dict>
			<key>@ㅇ</key>
			<string>deleteLine:</string>
			<key>@d</key>
			<string>deleteLine:</string>
		</dict>
		<key>Version</key>
		<integer>3</integer>
	</dict>
```

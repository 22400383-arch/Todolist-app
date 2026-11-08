Project Structure: App.jsx- 앱의 Ui 및 기본 코드를 담당하는 파일. / App.css- 앱의 style을 담당하는 파일.
React Component: App.jsx 에서 form UI로 데이터를 입력받고 CRUD기능을 실행한다.
Code Analysis: 
const addTask = () => {
    if (task.trim() !== "") { 
      setTasks([...tasks, { text: task, category, dueDate }]);
      setTask("");
      setDueDate("");
    }
  };
입력받은 task에 공백이없다면 함수를 실행한다. 이전에 입력받은 task들과 새로 입력받은 데이터를 합친다. 그 후 입력받을 칸을 다시 공백으로 초기화한다. 

수정한 부분: 
Text- 입력받는 form의 라벨 및 placeholder를 한국어로 변경함. 버튼의 이름 또한 한글로 변경.
Style- Button, button-hover의 색을 변경함.
UI- 할 일 제목을 입력받는 input의 제목을 추가함
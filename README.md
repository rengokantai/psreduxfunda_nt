# psreduxfunda_nt
## 3. React Crash Course
### 3 React Hello World
```
npm install --save-dev babel-plugin-transform-react-jsx
```
```
babel --plugins transform-react-jsx js/new.js
```

### 4 React Scoreboard
```
class Score extends React.component{
  cpmstructor(props){
    super(props);
    this.state={score:0};
  }
  incrementScore(){
    this.setState({score:this.state.score+1;})
  }
  render(){
    return(
      <div>
      Score:{this.state.score}
        <button onClick={this.incrementScore}>+</button>
        <button>-</button>
      </div>
    )
  }
}
```

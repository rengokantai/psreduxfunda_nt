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
    this.incrementScore = this.increment.bind(this);
    
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

### 5 React and Webpack
```
"scripts":{
  "start":"webpack-dev-server --inline --output-public-path '/public/js/build'",
  "build":"webpack -p",
  "test":"echo \"error\" && exit 1"
}
```

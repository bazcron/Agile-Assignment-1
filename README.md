# Agile-Assignment-1

Name of webApp: Agree or Disagree

Created by: Barry Cronin Student Num: 20074828 
github link to project: https://github.com/bazcron/Agile-Assignment-1

This is my API test automation & Source Control Project.

Using my original webApp code for AgreeORdisagree i implemented tests for the 2 models i currently have,
Statements and Users.

Statements Model:
let mongoose = require('mongoose');
let statementSchema = new mongoose.Schema({
        id: Number,
        statement: String,
        agree: Number,
        disagree:Number
    },
    { collection: 'statements' });
module.exports = mongoose.model('statements', statementSchema);

Users Model:
let mongoose = require('mongoose');
let usersSchema = new mongoose.Schema({
        id: Number,
        name: String,
        email: String,
        password: String,
        agree: Number,
        disagree: Number
    },
    { collection: 'users' });
module.exports = mongoose.model('users', usersSchema);


I opened a terminal and set up an initial git repository inside the project folder: git init




References: https://moodle.wit.ie/course/view.php?id=163135&section=7

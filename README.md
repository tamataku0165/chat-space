# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|name|   |null: false|
|mail|    |null: false, unique: true|
|password|    |null: false|

### Association


## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|body|    |null: false|
|image|
|user_id|integer|
|group-id|integer|

### Association


## groupテーブル

|Column|Type|Options|
|------|----|-------|
|groupname|     |null: false, unique: true|
|user_id|integer|

### Association



## users_groupsテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|integer|
|group_id|integer|

### Association

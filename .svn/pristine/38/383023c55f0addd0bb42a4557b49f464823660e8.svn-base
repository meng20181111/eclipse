package com.demo.serviceimpl;

import java.util.Collections;
import java.util.List;

import org.apache.log4j.Logger;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

import com.demo.bean.Student;
import com.demo.dao.UserDao;
import com.demo.service.UserService;
@Service
public class UserServiceImpl implements UserService {
	
	private final static Logger l=Logger.getLogger(UserServiceImpl.class);
	@Autowired
	private UserDao us;
	@Override
	public List<Student> getAll() {
	List<Student> list=Collections.emptyList();
	
	try {
		list=us.getAll();
		l.info("查询全部学生数据----");
	} catch (Exception e) {
		l.info("查询全部学生数据-异常 ---e="+e);
		// TODO Auto-generated catch block
		e.printStackTrace();
	}
		return list;
	}

}

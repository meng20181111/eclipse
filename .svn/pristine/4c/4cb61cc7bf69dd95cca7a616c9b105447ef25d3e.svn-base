package com.demo.controller;

import java.util.ArrayList;
import java.util.List;

import javax.servlet.http.HttpServletRequest;

import org.apache.log4j.Logger;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

import com.demo.bean.Student;
import com.demo.service.UserService;

@Controller
@RequestMapping("/user")
public class                                                                       UserControlelr {

	private final static Logger l=Logger.getLogger(UserControlelr.class);
	@Autowired
	private UserService us;
	@RequestMapping("all")
	public String getAll(HttpServletRequest request, Model model){
		List<Student> list=new ArrayList<>();
	list=	us.getAll();
	
	l.info("list.size()="+list.size());
	model.addAttribute("List", list);
		
		return "student";
		
	}
	
}
